---
book: ens
book_title: Theory of Sets
chapter: III
chapter_title: ORDERED SETS, CARDINALS, INTEGERS
section: 7
section_title: Inverse limits and direct limits
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 191-211, 251-254
pdf_pages: 0197-0217, 0257-0260
extraction: ocr
subsections:
    - "no": 1
      title: INVERSE LIMITS
      page: 191
      pdf_page: 197
    - "no": 2
      title: INVERSE SYSTEMS OF MAPPINGS
      page: 192
      pdf_page: 198
    - "no": 3
      title: DOUBLE INVERSE LIMIT
      page: 196
      pdf_page: 202
    - "no": 4
      title: CONDITIONS FOR AN INVERSE LIMIT TO BE NON-EMPTY
      page: 198
      pdf_page: 204
    - "no": 5
      title: DIRECT LIMITS
      page: 202
      pdf_page: 208
    - "no": 6
      title: DIRECT SYSTEMS OF MAPPINGS
      page: 204
      pdf_page: 210
    - "no": 7
      title: DOUBLE DIRECT LIMIT. PRODUCT OF DIRECT LIMITS
      page: 209
      pdf_page: 215
statements: 34
exercises: 9
errata:
    - says: no. 2, Proposition 2, Corollary 2
      read: no. 2, Proposition 1, Corollary 2
      why: The fact cited on page 197 is that the maps of an inverse system compose, h to the lambda nu being h to the lambda mu after h to the mu nu, and that is Corollary 2 of Proposition 1 of no. 2, the corollary on three inverse systems. Proposition 2 of that no. prints one corollary and it carries no number.
content_sha256: eb31c31e3d763a7188ba150801655dbc55e11a31b7881ee8bba1194956d1e3d0
translated_from: content/en/ens/III/07_s7_inverse_limits_and_direct_limits.md
translation_method: google
source_content_sha256: 32f34a0e7e91e7e94cb6dacf6471b60fe7158e208c5d0e1bd2901e3f619ccda7
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 70a315fbaa758b544d0d6cfdbf633b1a4567abde8811c2cc1daae94c90224253
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 7. 逆極限および正極限

### 1. インバース極限

$I$ を事前注文された集合とし、$(E_\alpha)_{\alpha\in I}$ を $I$ によってインデックス付けされた集合のファミリーとします。 $\alpha\leq\beta$ となるような $I$ の元の各対 $(\alpha,\beta)$ について、$f_{\alpha\beta}$ を $E_\beta$ の写像から $E_\alpha$ にします。 $f_{\alpha\beta}$ 満たすが次の条件であると仮定します。

$(\mathrm{LP}_I)$ *関係 $\alpha\leq\beta\leq\gamma$ は $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$ を暗示します。*

$(\mathrm{LP}_{II})$ *それぞれの $\alpha\in I$、$f_{\alpha\alpha}$ は $E_\alpha$ の恒等写像です。

$G=\prod_{\alpha\in I}E_\alpha$ を集合 $(E_\alpha)_{\alpha\in I}$ の家族の *積* とし、$E$ を $G$ からなるの $x$ の部分集合と、それぞれ満たすを表すとします。 関係

(1)

$$\operatorname{pr}_{\alpha}x=f_{\alpha\beta}(\operatorname{pr}_{\beta}x)$$

添字 $(\alpha,\beta)$ の各対に対して、$\alpha\leq\beta$ になります。 $E$ は、写像* $(f_{\alpha\beta})$ の家族に関して、家族* $(E_\alpha)_{\alpha\in I}$ の *逆数極限であると言われており、曖昧さの危険がない場合は、$E=\underset{\longleftarrow}{\lim}\,(E_\alpha,f_{\alpha\beta})$ または単に $E=\underset{\longleftarrow}{\lim}\,E_\alpha$ と書きます。言葉の乱用により、対 $((E_\alpha),(f_{\alpha\beta}))$ (通常は $(E_{\alpha\beta},f_{\alpha\beta})$ で示される) は、添字集合 $I$ に対して、集合* の *逆系と呼ばれます。 射影 $\operatorname{pr}_\alpha$ から $E$ の *制限* $f_\alpha$ は、$E$ から $E_\alpha$ の *標準写像* と呼ばれ、関係になります

(2)

$$f_\alpha=f_{\alpha\beta}\circ f_\beta$$

いつでも $\alpha\leq\beta$;これは、定義する $E$ 関係 (1) を転写したものにすぎません。

*例*

#### 例 1 {#ens-iii-s7-n1-exa-1 .statement tag=03TF}

$I$ の順序関係が *等式* の関係であるとします。すると、$\alpha\leq\beta$ となる唯一の対 $(\alpha,\beta)$ は対 $(\alpha,\alpha)$ ここで $\alpha\in I$;そして、$f_{\alpha\alpha}$ は恒等写像であるため、関係 (1) は *すべて* $x\in G$ に対して満たされます。他の語では、$\underset{\longleftarrow}{\lim}\,E_\alpha$ は *積* $\prod_{\alpha\in I}E_\alpha$ になります。

#### 例 2 {#ens-iii-s7-n1-exa-2 .statement tag=03TG}

$I$ が *右向き* であり、$E_\alpha$ がすべての $\alpha\in I$ に対して同じ集合 $F$ であり、$f_{\alpha\beta}$ が $\alpha\leq\beta$ になるたびに$F$ の恒等写像であると仮定します。すると、$E=\underset{\longleftarrow}{\lim}\,E_\alpha$ は積 $\prod_{\alpha\in I}E_\alpha=F^I$ の *対角* $\Delta$ です。実際、それぞれの $x\in\Delta$ が関係 (1) を満たすことは明らかです。逆に、$x$ を $E$ の元とし、添字 $(\alpha, \beta)$ の各対に対して $\mathrm{pr}_\alpha x = \mathrm{pr}_\beta x$ があることを示します。 仮定までに、$\alpha \leqslant \gamma$ と $\beta \leqslant \gamma$ のような添字 $\gamma \in I$ が存在します。したがって、(1) によって $\mathrm{pr}_\alpha x = f_{\alpha\gamma}(\mathrm{pr}_\gamma x) = \mathrm{pr}_\gamma x$ が得られ、同様に $\mathrm{pr}_\beta x = \mathrm{pr}_\gamma x$ が得られ、これにより主張が証明されます。

すべての $E_\alpha$ が空でなく、すべての写像 $f_{\alpha\beta}$ が *全射* である場合でも、$E = \varprojlim E_\alpha$ は *空* になる可能性があることに注意してください (練習問題 4; no. 4 を参照)。

¶ サブファミリー $(E_\alpha)_{\alpha \in J}$ およびファミリー $(f_{\alpha\beta})$ の I 対からなるの各部分集合 J について、$\alpha \in J$、$\beta \in J$、および $\alpha \leqslant \beta$ が再び逆数であることは明らかです。 J に対する集合の系;それは、添字集合を J に *制限することによって得られると言われています。 E と E' がそれぞれ、家族 $(E_\alpha)_{\alpha \in I}$ と $(E_\alpha)_{\alpha \in J}$ の逆数極限を表すものとします。それぞれ $x \in E$ 元

$$g(x) = (f_\alpha(x))_{\alpha \in J} \tag{3}$$

(2) により E' に属する;このように定義された写像 $g : E \to E'$ は *正規* と呼ばれます。 J' が J の部分集合で、E'' が族 $(E_\alpha)_{\alpha \in J'}$ の逆数極限で、$g' : E' \to E''$ と $g'' : E \to E''$ が標準写像である場合、定義によって次のようになります。

$$g'' = g' \circ g. \tag{4}$$

### 2. 写像の逆系

#### 命題 1 {#ens-iii-s7-prop-1 .statement tag=03OC}

*I *を順序付き集合とし、* $(E_\alpha, f_{\alpha\beta})$ *Iを基準とした集合の逆数系とし、*$E = \varprojlim E_\alpha$ *その逆数極限とし、それぞれ* $\alpha \in I$ *let*

$$f_\alpha : E \to E_\alpha$$

*標準写像になります。それぞれ* $\alpha \in I$ に対して、*$u_\alpha$ *be 写像 of 集合* F *into* $E_\alpha$ *そのような*

$$f_{\alpha\beta} \circ u_\beta = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta. \tag{5}$$

*それでは:*

(a) *ある一意な写像* $u$ *の* F *が* E *そのような*

$$u_\alpha = f_\alpha \circ u \qquad \textit{for all } \alpha \in I;\tag{6}$$

(b) *写像* $u$ *は、個別の元* $y$、$z$ *F の各対に対して、 *$\alpha \in I$ *そのような* $u_\alpha(y) \neq u_\alpha(z)$ が存在する*場合に限り、単射法です。

関係 $u_\alpha = f_\alpha \circ u$ は、各 $y \in F$ について、

$$\mathrm{pr}_\alpha(u(y)) = u_\alpha(y);$$

元 $u(y) \in \prod_{\alpha \in I} E_\alpha$ は $u(y) = (u_\alpha(y))_{\alpha \in I}$ によって一意に決まります。すべての $y \in F$ に対して $u(y) \in E$ が、他の語において、

$$\mathrm{pr}_\alpha(u(y)) = f_{\alpha\beta}(\mathrm{pr}_\beta(u(y)))$$

いつでも$\alpha \leqslant \beta$。しかし、これは形で書くことができます。

$$u_\alpha(y) = f_{\alpha\beta}(u_\beta(y))$$

したがって、(5) から導かれます。 命題の 2 番目の部分は、定義の直後に続きます。

#### 系 1 {#ens-iii-s7-prop-1-cor-1 .statement tag=03RN}

*$(E_\alpha, f_{\alpha\beta})$ * と * $(F_\alpha, g_{\alpha\beta})$ * を、同じ添字集合* I に対する集合の 2 つの逆数系とします。 * $E = \varprojlim E_\alpha$、$F = \varprojlim F_\alpha$、*そして* $f_\alpha$ *(それぞれ* $g_\alpha$*) 標準写像 of* E *into* $E_\alpha$ *(それぞれ* F *into* $F_\alpha$*) $\alpha \in I$、*それぞれ* $\alpha \in I$, *$u_\alpha$ *を* E *の写像に* $F_\alpha$ *図式*になるように

$$\begin{array}{ccc} E_\beta & \overset{u_\beta}{\longrightarrow} & F_\beta \\ {\scriptstyle f_{\alpha\beta}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\alpha\beta}} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*可換です* [^1] *いつでも* $\alpha \leqslant \beta$。 *その後、 一意な写像* $u : E \to F$ *それぞれについて* $\alpha \in I$ *図式* が存在します

$$\begin{array}{ccc} E & \overset{u}{\longrightarrow} & F \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ E_\alpha & \underset{u_\alpha}{\longrightarrow} & F_\alpha \end{array}$$

*は可換です。*

$v_\alpha = u_\alpha \circ f_\alpha$を入れてください。 $\alpha \leqslant \beta$ の場合、(2) により、

$$g_{\alpha\beta} \circ v_\beta = g_{\alpha\beta} \circ u_\beta \circ f_\beta = u_\alpha \circ f_{\alpha\beta} \circ f_\beta = u_\alpha \circ f_\alpha = v_\alpha,$$

したがって、命題を適用する 1 から写像 $v_\alpha$ になります。したがって、写像 $u:E\to F$ の存在と一意性は次のようになります。

$$
g_\alpha\circ u=v_\alpha=u_\alpha\circ f_\alpha
$$

それぞれの$\alpha\in I$。

¶ 系 1 の条件を満たす写像 $u_\alpha:E_\alpha\to F_\alpha$ の族は、$(E_\alpha,f_{\alpha\beta})$ の写像* を $(F_\alpha,g_{\alpha\beta})$ に * 逆数系と呼ばれます。 系 1 で定義された写像 $u$ は、族 $(u_\alpha)$ の *逆数極限* と呼ばれ、混乱の危険がない場合は $u=\underset{\leftarrow}{\lim}\,u_\alpha$ と書かれます。

#### 系 2 {#ens-iii-s7-prop-1-cor-2 .statement tag=03RO}

$(E_\alpha,f_{\alpha\beta})$、$(F_\alpha,g_{\alpha\beta})$、$(G_\alpha,h_{\alpha\beta})$ を、同じ添字集合* $I$ に対する集合の 3 *逆数系とします。 $E=\underset{\leftarrow}{\lim}\,E_\alpha$、$F=\underset{\leftarrow}{\lim}\,F_\alpha$、$G=\underset{\leftarrow}{\lim}\,G_\alpha$、そして$f_\alpha$ (それぞれ $g_\alpha,h_\alpha$) を $E$ (それぞれ $F,G$) の *標準写像* として $E_\alpha$ (それぞれ $F_\alpha,G_\alpha$) に加えます。 $(u_\alpha)$ と $(v_\alpha)$ が写像*、$u_\alpha:E_\alpha\to F_\alpha$、$v_\alpha:F_\alpha\to G_\alpha$ の *2 つの逆数系である場合、*合成写像* $v_\alpha\circ u_\alpha:E_\alpha\to G_\alpha$ 形は *逆数系写像*、そして私たちは

(7)

$$
\underset{\leftarrow}{\lim}\,(v_\alpha\circ u_\alpha)
=
\left(\underset{\leftarrow}{\lim}\,v_\alpha\right)\circ
\left(\underset{\leftarrow}{\lim}\,u_\alpha\right).
$$

というのは、$w_\alpha=v_\alpha\circ u_\alpha$ とすると、$\alpha\leq\beta$ とすると、

$$
w_\alpha\circ f_{\alpha\beta}
=v_\alpha\circ(u_\alpha\circ f_{\alpha\beta})
=v_\alpha\circ(g_{\alpha\beta}\circ v_\beta)
=(h_{\alpha\beta}\circ v_\beta)\circ u_\beta
=h_{\alpha\beta}\circ w_\beta,
$$

これは、$(w_\alpha)$ が写像の逆数系であることを示しています。さらに、$u=\underset{\leftarrow}{\lim}\,u_\alpha$と$v=\underset{\leftarrow}{\lim}\,v_\alpha$の場合、それぞれの$\alpha\in I$に対して$h_\alpha\circ(v\circ u)=(v_\alpha\circ g_\alpha)\circ u=(v_\alpha\circ u_\alpha)\circ f_\alpha$、したがって、極限の逆数の一意性により、$v\circ u=\underset{\leftarrow}{\lim}\,w_\alpha$が得られます。

¶ $(E_\alpha,f_{\alpha\beta})$ を集合の逆数系とし、各 $\alpha\in I$ について $M_\alpha$ を $E_\alpha$ の部分集合とします。 $\alpha\leq\beta$ のときはいつでも $f_{\alpha\beta}(M_\beta)\subset M_\alpha$ であれば、$M_\alpha$ は $E_\alpha$ の部分集合* の * 逆数系である形と言われます。 $g_{\alpha\beta}$ を $M_\beta$ の写像から $M_\alpha$ ($\alpha\leq\beta$) にすると、そのグラフは $f_{\alpha\beta}$ から $M_\beta$ の制限のグラフと同じになります。次に、$(M_\alpha,g_{\alpha\beta})$ が集合の逆数系であることは明らかです。

(8)

$$
\underset{\leftarrow}{\lim}\,M_\alpha
=
\left(\underset{\leftarrow}{\lim}\,E_\alpha\right)\cap\prod_{\alpha\in I}M_\alpha.
$$

#### 命題 2 {#ens-iii-s7-prop-2 .statement tag=03RP}

$(E_\alpha,f_{\alpha\beta})$ と $(E'_\alpha,f'_{\alpha\beta})$ を $I$ に対する 2 つの *逆集合系* とし、 $u_\alpha$ を $\alpha\in I$ ごとに $E_\alpha$ から $E'_\alpha$ への写像とし、$u_\alpha$ が *逆写像系 * を形成するようにします。 $u=\underset{\leftarrow}{\lim}\,u_\alpha$ にしましょう。 次に、各 $x'=(x'_\alpha)\in E'=\underset{\leftarrow}{\lim}\,E'_\alpha$、$\bar u_\alpha^{-1}(x'_\alpha)$ 形について、$E_\alpha$、$\bar u^{-1}(x')=\underset{\leftarrow}{\lim}\,\bar u_\alpha^{-1}(x'_\alpha)$ の部分集合* の * 逆数系です。

$\alpha \leqslant \beta$ と $x_\beta \in \overset{-1}{u_\beta}(x'_\beta)$ の場合、

$$u_\alpha(f_{\alpha\beta}(x_\beta)) = f'_{\alpha\beta}(u_\beta(x_\beta)) = f'_{\alpha\beta}(x'_\beta) = x'_\alpha,$$

最初の主張が続きます。そして、$x = (x_\alpha) \in \mathrm{E} = \varprojlim \mathrm{E}_\alpha$ が $u(x) = x'$ であると言うことは、定義によって、各 $\alpha \in \mathrm{I}$ に対して $u_\alpha(x_\alpha) = x'_\alpha$ を意味します。

#### 系 {#ens-iii-s7-n2-cor-1 .statement tag=03OD}

*各 $\alpha \in \mathrm{I}$ に対して $u_\alpha$ が単射* (それぞれ *全単射*) である場合、 $u$ は単射* (それぞれ *全単射*) です。

命題 2 の記法、像 $u_\alpha(\mathrm{E}_\alpha)$ も形 $\mathrm{E}'_\alpha$ の部分集合の逆数系で、次のようになります。

(9) $$u(\mathrm{E}) \subset \varprojlim u_\alpha(\mathrm{E}_\alpha);$$

しかし、この関係の 2 つの辺は *必ずしも等しいわけではありません* (練習問題 4)。

#### 命題 3 {#ens-iii-s7-prop-3 .statement tag=03OE}

*$\mathrm{I}$ を事前注文された集合とし、$(\mathrm{E}_\alpha, f_{\alpha\beta})$ を $\mathrm{I}$ に対する集合の逆数系とし、$\mathrm{E} = \varprojlim \mathrm{E}_\alpha$ とします。 $\mathrm{J}$ を $\mathrm{J}$ が右向きとなるような $\mathrm{I}$ の余終点部分集合とし、$\mathrm{E}'$ を添字を制限して $(\mathrm{E}_\alpha, f_{\alpha\beta})$ から得られる集合の逆数系の逆数極限とする。 集合から$\mathrm{J}$まで。次に、$\mathrm{E}$ の標準写像 $g$ を $\mathrm{E}'$* (no. 1, *公式* (3)) *全単射*です。

それぞれの $\alpha \in \mathrm{J}$ について、$f'_\alpha$ を標準写像 $\mathrm{E}' \to \mathrm{E}_\alpha$ とします。次に、(2) と (5) により、$g$ は $\mathrm{E}$ の一意な写像を $\mathrm{E}'$ に変換し、すべての $\alpha \in \mathrm{J}$ に対して $f_\alpha = f'_\alpha \circ g$ (命題 1) となります。 命題 1 の基準を使用して、$g$ が単射であることを示します。$x$、$y$ が $\mathrm{E}$ の元である場合、定義までに $f_\alpha(x) \neq f_\alpha(y)$ となるような $\alpha \in \mathrm{I}$ が存在します。 $\mathrm{J}$ は $\mathrm{I}$ の最終であるため、$\alpha \leqslant \lambda$ となるような $\lambda \in \mathrm{J}$ が存在します。 $f_{\alpha\lambda}(f_\lambda(x)) \neq f_{\alpha\lambda}(f_\lambda(y))$ から、$f_\lambda(x) \neq f_\lambda(y)$ になります。 $g$ が全射であることはまだ証明されていません。 $x' = (x'_\lambda)_{\lambda \in \mathrm{J}}$を$\mathrm{E}'$の元とします。それぞれの $\alpha \in \mathrm{I}$ には、$\alpha \leqslant \lambda$ となるような $\lambda \in \mathrm{J}$ が存在し、元 $f_{\alpha\lambda}(x'_\lambda)$ は $\alpha \leqslant \lambda$ となるような添字 $\lambda \in \mathrm{J}$ に依存しません。なぜなら、$\mu \in \mathrm{J}$が$\alpha \leqslant \mu$である場合、$\lambda \leqslant \nu$と$\mu \leqslant \nu$である$\nu \in \mathrm{J}$が存在するため、$f_{\alpha\lambda}(x'_\lambda) = f_{\alpha\lambda}(f_{\lambda\nu}(x'_\nu)) = f_{\alpha\nu}(x'_\nu)$、そして同様に$f_{\alpha\mu}(x'_\mu) = f_{\alpha\nu}(x'_\nu)$が存在します。 $x_\alpha$ を $\lambda \in \mathrm{J}$ の $f_{\alpha\lambda}(x'_\lambda)$ の共通の値として、$\alpha \leqslant \lambda$ とし、$x = (x_\alpha)_{\alpha \in \mathrm{I}}$ とします。次に $x \in \mathrm{E}$ です。なぜなら、$\alpha \leqslant \beta$ と $\lambda \in \mathrm{J}$ が $\beta \leqslant \lambda$ である場合、次のようになります。

$$f_{\alpha\beta}(x_\beta) = f_{\alpha\beta}(f_{\beta\lambda}(x'_\lambda)) = f_{\alpha\lambda}(x'_\lambda) = x_\alpha.$$

最後に、すべての $\lambda \in \mathrm{J}$ に対して $x'_\lambda = f_{\lambda\lambda}(x'_\lambda)$ が得られるため、すべての $\lambda \in \mathrm{J}$ に対して $x_\lambda = x'_\lambda$ が得られます。他の語、$f(x_\lambda) = x'_\lambda$、つまり$g(x) = x'$。したがって、$g$ は全射法であり、証明は完全です。

特に、$\mathrm{I}$ に *最大の元* $\omega$ がある場合、$\mathrm{J} = \{\omega\}$ を採用して、$\varprojlim \mathrm{E}_\alpha$ が正規に $\mathrm{E}_\omega$ と識別されるようにします。

*注意*

#### 注意 1 {#ens-iii-s7-n2-rem-1 .statement tag=03TH}

それぞれの $\alpha \in I$ に $E'_\alpha = f_\alpha(E)$ を入れます。次に、(2) の理由により、集合 $E'_\alpha$ 形は、$E_\alpha$ の部分集合* の * 逆数系となり、$\varprojlim E'_\alpha = E = \varprojlim E_\alpha$ であることはすぐに明らかです。 写像 $f'_{\alpha\beta} : E'_\beta \to E'_\alpha$ ($\alpha \leqslant \beta$) のグラフは $f_{\alpha\beta}$ から $E_\beta$ の制限と同じであり、*全射* であり、次のようになります。

$$(10) \qquad E'_\alpha = f_\alpha(E) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(E_\beta)$$

すべての$\alpha \in I$に。

#### 注意 2 {#ens-iii-s7-n2-rem-2 .statement tag=03TI}

I を (*正しい*) *有向 * 順序の集合とし、$(E_\alpha, f_{\alpha\beta})$ を I に対する集合の逆数系とし、それぞれの $\alpha \in I$ について、$u_\alpha : F \to E_\alpha$ を写像とします。 $(u_\alpha)$ は公式 (5) を満たします。 I によってインデックス付けされた逆系 $(F_\alpha, i_{\alpha\beta})$ を考えます。ここで、すべての $\alpha \in I$ と $i_{\alpha\beta}$ の $F_\alpha = F$ は F の恒等写像です。すると、(no. 1, 例 2) F は正規的に $\varprojlim F_\alpha$ と識別されます。 $u_\alpha$を$F_\alpha$の写像を$E_\alpha$にすると考えると、$(u_\alpha)$は写像の逆数系であり、(6)で定義される写像$u : F \to E$はこれの逆数極限と同一視されます。 写像の系。従って、言葉の乱用により、$u = \varprojlim u_\alpha$と書きます。

#### 注意 3 {#ens-iii-s7-n2-rem-3 .statement tag=03TJ}

I を順序付き集合とし、$(E_\alpha, f_{\alpha\beta})$ を I に対する集合の逆数系とします。 I の各有限部分集合 J について、添字集合を J に制限することによって、$(E_\alpha, f_{\alpha\beta})$ から得られる (有限) 逆数系の逆数極限を$F_J$ とします。 J と K が $J \subset K$ となるような I の任意の 2 つの有限部分集合である場合、$g_{JK}$ は $F_K$ の標準写像 (3) を $F_J$ に表すものとします。 次に、関係 (4) は、$(F_J, g_{JK})$ が、I の有限部分集合の *指示* 集合 (関係 $\subset$ に関して) $\mathfrak{F}(I)$ に対して、集合の *逆系* であることを示します。 次に、それぞれの $J \in \mathfrak{F}(I)$ について、$h_J : E \to F_J$ を標準写像とします (3)。 (4) と、注意 (2) で述べた言葉の乱用により、$(h_J)$ は写像の *逆系* になります。 $h = \varprojlim h_J : E \to F = \varprojlim F_J$ を置き、$h$ が *全単射* (*正規* と呼ばれる) であることを示しましょう。 確かに、$y = (y_J) \in F$ としましょう。 定義までに $y_J = (x_{\alpha, J})_{\alpha \in J}$ があり、すべての $\alpha \in J$ に対して $x_{\alpha, J} \in E_\alpha$ になります。 $J \subset K$ の場合、写像 $g_{JK}$ の定義により、$y_J = g_{JK}(y_K)$ なので、すべての $\alpha \in J$ に対して $x_{\alpha, J} = x_{\alpha, K}$ が得られます。 従って、$\alpha \in I$ が与えられると、含む $\alpha$ である I のすべての有限部分集合 J に対して $x_\alpha = x_{\alpha, J}$ となるような一意元 $x_\alpha \in E_\alpha$ が存在します。 $\alpha \leqslant \beta$ の場合、$\alpha$ と $\beta$ の両方含むである I の有限部分集合 J があります。従って、$x_\alpha = f_{\alpha\beta}(x_\beta)$ by 定義。 従って、$x = (x_\alpha)$ は、$h(x) = y$ となる E の一意元です。

### 3. ダブルインバース極限

I、L を 2 つの予約済み集合、$I \times L$ の積 (§ 1, no. 4) とします。 添字集合 $I \times L$ に対する集合 $(E^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ の逆数系を考えてみましょう。

我々は持っています

(11) $\alpha \leqslant \beta \leqslant \gamma$ と $\lambda \leqslant \mu \leqslant \nu$ の場合は常に $\qquad f^{\lambda\nu}_{\alpha\gamma} = f^{\lambda\mu}_{\alpha\beta} \circ f^{\mu\nu}_{\beta\gamma}$。

E または $\lim \mathrm{E}^{\lambda}_{\alpha}$ がこの逆数系の逆数極限を表すものとします。

それぞれの $\lambda \in \mathrm{L}$ に $g^{\lambda}_{\alpha\beta} = f^{\lambda\lambda}_{\alpha\beta} : \mathrm{E}^{\lambda}_{\beta} \to \mathrm{E}^{\lambda}_{\alpha}$ を入れます。 (11) から次のことがわかります。

(12) $\alpha \leqslant \beta \leqslant \gamma$ のたびに $\qquad g^{\lambda}_{\alpha\gamma} = g^{\lambda}_{\alpha\beta} \circ g^{\lambda}_{\beta\gamma}$、

したがって、$(\mathrm{E}^{\lambda}_{\alpha}, g^{\lambda}_{\alpha\beta})$ は I を基準とした集合の逆数系になります。 $\mathrm{F}^{\lambda} = \lim \mathrm{E}^{\lambda}_{\alpha}$ がその逆数極限を表すものとします。 L の固定 $\lambda \leqslant \mu$ の場合、(11) から、$h^{\lambda\mu}_{\alpha} = f^{\lambda\mu}_{\alpha\alpha} : \mathrm{E}^{\mu}_{\alpha} \to \mathrm{E}^{\lambda}_{\alpha}$ 形は写像の逆数系となり、その逆数極限を $h^{\lambda\mu} = \lim h^{\lambda\mu}_{\alpha} : \mathrm{F}^{\mu} \to \mathrm{F}^{\lambda}$ で表します。 L で $\lambda \leqslant \mu \leqslant \nu$ の場合、

(13) $$h^{\lambda\nu} = h^{\lambda\mu} \circ h^{\mu\nu}$$

(no. 2、命題 2、系 2);したがって、$(\mathrm{F}^{\lambda}, h^{\lambda\mu})$ は、L に対する集合の逆数系です。 $\mathrm{F} = \lim \mathrm{F}^{\lambda}$ をその逆数極限とします。 定義するを *正規の全単射* $\mathrm{F} \to \mathrm{E}$ とします。これを行うには、F が $\prod_{\lambda \in \mathrm{L}} \mathrm{F}^{\lambda}$ の定義部分集合であり、$\mathrm{F}^{\lambda}$ が $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$ の部分集合であることに注意します。したがって、F は、$\prod_{(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}} \mathrm{E}^{\lambda}_{\alpha} = \mathrm{G}$ の部分集合 (章 II, § 5, no. 5、命題 7) と正規的に識別される可能性があります。それぞれの $z \in \mathrm{G}$ について、$\mathrm{pr}^{\lambda}(z)$ は $\prod_{\alpha \in \mathrm{I}} \mathrm{E}^{\lambda}_{\alpha}$ の元 $(\mathrm{pr}^{\lambda}_{\alpha}(z))_{\alpha \in \mathrm{I}}$ を表します。そして、もし、そしてその場合に限り、$z \in \mathrm{F}$

(14) L で $\lambda \leqslant \mu$ になるたびに $\qquad \mathrm{pr}^{\lambda}(z) = h^{\lambda\mu}(\mathrm{pr}^{\mu}(z))$

すべての $\lambda \in \mathrm{L}$ に対して $\mathrm{pr}^{\lambda}(z) \in \mathrm{F}^{\lambda}$。つまり、$\alpha \leqslant \beta$ が I になるたびに、

(15) $$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\lambda}_{\alpha\beta}(\mathrm{pr}^{\lambda}_{\beta}(z)).$$

しかし、$h^{\lambda\mu}(\mathrm{pr}^{\mu}(z)) = (f^{\mu\lambda}_{\alpha\alpha}(\mathrm{pr}^{\mu}_{\alpha}(z))_{\alpha \in \mathrm{I}}$;したがって、(14) と (15) から、$\alpha \leqslant \beta$ と $\lambda \leqslant \mu$ の場合、次のようになります。

$$\mathrm{pr}^{\lambda}_{\alpha}(z) = f^{\lambda\mu}_{\alpha\alpha}(f^{\mu\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z))) = f^{\lambda\mu}_{\alpha\beta}(\mathrm{pr}^{\mu}_{\beta}(z)),$$

これは $z \in \mathrm{E}$ を意味します。 逆は明らかなので、次のことを証明しました。

#### 命題 4 {#ens-iii-s7-prop-4 .statement tag=03OF}

*もし* $(\mathrm{E}^\lambda_\alpha, f^{\lambda\mu}_{\alpha\beta})$ * が、事前注文された集合の積* $\mathrm{I} \times \mathrm{L}$ に対する集合の逆数系である場合、(正規の全単射まで)*

$$(16) \qquad \varprojlim_{\alpha,\lambda} \mathrm{E}^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

#### 系 1 {#ens-iii-s7-prop-4-cor-1 .statement tag=03OG}

*$(\mathrm{{E}'}^\lambda_\alpha, {f'}^{\mu\lambda}_{\alpha\beta})$ *他のを $\mathrm{I} \times \mathrm{L}$ を基準にして集合の逆系にします。 *それぞれについて* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *$u^\lambda_\alpha$ *写像を * $\mathrm{E}^\lambda_\alpha$ *into* $\mathrm{{E}'}^\lambda_\alpha$ *次のようにします* $u^\lambda_\alpha$ *形写像の逆系。それから*

$$(17) \qquad \varprojlim_{\alpha,\lambda} u^\lambda_\alpha = \varprojlim_\lambda \; (\varprojlim_\alpha u^\lambda_\alpha).$$

検証は命題 4 と同様です。

#### 系 2 {#ens-iii-s7-prop-4-cor-2 .statement tag=03OH}

*$(\mathrm{E}^\lambda_\alpha, f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$ * を、* I に対する集合の逆数系の族とします。 *もし* $\prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta}$ * が拡大から積* (章 II, § 5, no. 7, 定義 2) * 写像* $(f^\lambda_{\alpha\beta})_{\lambda \in \mathrm{L}}$ の場合、 *その場合* $\left( \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha, \prod_{\lambda \in \mathrm{L}} f^\lambda_{\alpha\beta} \right)$ * はその逆数系集合を * I と比較し、*そして (正規の全単射まで)*

$$(18) \qquad \varprojlim_\alpha \prod_{\lambda \in \mathrm{L}} \mathrm{E}^\lambda_\alpha = \prod_{\lambda \in \mathrm{L}} (\varprojlim_\alpha \mathrm{E}^\lambda_\alpha).$$

$\mathrm{I} \times \mathrm{L}$ に対する二重逆数系 $(\mathrm{E}^\lambda_\alpha, g^{\lambda\mu}_{\alpha\beta})$ を考えてみましょう。ここで、L の順序関係は等式 (no. 1, 例 1)、命題を適用する 4 です。

### 4. 条件逆数極限が空でない場合

この小節では、逆行列極限が空でないために最も頻繁に使用される 2 つの条件を与えます (練習問題 5 も参照)。

#### 命題 5 {#ens-iii-s7-prop-5 .statement tag=03OI}

*$(\mathrm{E}_\alpha, f_{\alpha\beta})$ * を、可算*余終値部分集合を持つ * 方向 * 集合* I に対する集合の逆数系とし、さらに* $f_{\alpha\beta}$ * が* 全射であると仮定します。 *次に、* $\mathrm{E} = \varprojlim \mathrm{E}_\alpha$、*標準写像* $f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$ * がそれぞれ* $\alpha \in \mathrm{I}$ * に対して全射である場合、* (そして、なおさら、* E * は空ではありません。ただし、* $\mathrm{E}_\alpha$ * が空ではありません)。

$(\alpha_n)$ を I の元の数列とし、形をI の最終部分集合とします。 I が指示されているので、$i < n$ と $\beta_n \geqslant \alpha_n$ に対して条件 $\beta_0 = \alpha_0, \beta_n \geqslant \beta_i$ によって帰納的に I の元の定義する数列 $(\beta_n)$ ができます。明らかに、数列 $(\beta_n)$ は増加すると形が I の最終部分集合です。 no. 1 の命題 1 と $\alpha \leqslant \beta_n$ の関係 $f_\alpha = f_{\alpha\beta_n} \circ f_{\beta_n}$ を考慮すると、$\mathrm{I} = \mathbf{N}$ の場合については命題を証明するだけで済みます。さらに、$f_0$ が全射であることを証明すれば十分であることは明らかです。 $x_0 \in \mathrm{E}_0$ にしましょう。 定義する $x_n \in \mathrm{E}_n$ ($n \geqslant 1$ の場合) は、帰納的に集合 $\overset{-1}{f}_{n-1,n}(x_{n-1})$ の元になります。これは、後者の集合が仮定によって空ではないため、可能です。次に、$n - m$ の帰納法によって $m \leqslant n$ の $x_m = f_{mn}(x_n)$ が示され、E に対して $x = (x_n)$ 属するが続きます。

2 番目の基準は、添字集合 I に対する逆系 $(\mathrm{E}_\alpha, f_{\alpha\beta})$ に関するもので、$\alpha \in \mathrm{I}$ ごとに $\mathrm{E}_\alpha$ の部分集合のうち集合 $\mathfrak{S}_\alpha$ が与えられ、次の満たすが与えられます。 条件 :

(i) *集合所属から $\mathfrak{S}_\alpha$ までの共通部分ごと、また属するから $\mathfrak{S}_\alpha$ まで。*

特に (空の家族の共通部分を考慮すると) $\mathrm{E}_\alpha \in \mathfrak{S}_\alpha$ になります。

(ii) *部分集合 $\mathfrak{F} \subset \mathfrak{S}_\alpha$ の集合が、集合所属から $\mathfrak{F}$ までのすべての有限共通部分が空でない場合、$\bigcap\limits_{\mathbf{M} \in \mathfrak{F}} \mathrm{M}$ は空ではありません。

(i) を考慮すると、(ii) が次の条件と同等であることは明らかです。

(ii)' *$\mathfrak{G} \subset \mathfrak{S}_\alpha$ が (包含に関して) 指示されたままで、含むが空の集合ではない場合、$\bigcap\limits_{\mathbf{M} \in \mathfrak{G}} \mathrm{M}$ は空ではありません。*

#### 定理 1 {#ens-iii-s7-thm-1 .statement tag=03RQ}

*I が方向付けされ、集合 $\mathfrak{S}_\alpha$ 満たす条件* (i) *および* (ii)、*そしてその逆系 $(\mathrm{E}_\alpha, f_{\alpha\beta})$ が次の特性を持つと仮定します。*

(iii) *添字 $\alpha$、$\beta$ の各対について、$\alpha \leqslant \beta$、および各 $x_\alpha \in \mathrm{E}_\alpha$ には、$\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ があります。*

(iv) *添字 $\alpha$、$\beta$ の各対について、$\alpha \leqslant \beta$、および各 $\mathrm{M}_\beta \in \mathfrak{S}_\beta$ には、$f_{\alpha\beta}(\mathrm{M}_\beta) \in \mathfrak{S}_\alpha$ があります。*

*それぞれの$\alpha \in \mathrm{I}$に対して、$\mathrm{E} = \varprojlim \mathrm{E}_\alpha$と$f_\alpha : \mathrm{E} \to \mathrm{E}_\alpha$を標準写像とします。それから：*

(a) *それぞれの $\alpha \in \mathrm{I}$ について*

$$(19) \qquad f_\alpha(\mathrm{E}) = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

(b) *各 $\alpha \in \mathrm{I}$ に対して $\mathrm{E}_\alpha$ が空でない場合、E は空ではありません。*

$\Sigma$ を、次の条件満たすを含む家族 $\mathfrak{A} = (\mathrm{A}_\alpha)_{\alpha \in \mathrm{I}}$ の集合とします。

$$(20) \qquad \mathrm{A}_\alpha \neq \emptyset \quad \textit{and} \quad \mathrm{A}_\alpha \in \mathfrak{S}_\alpha \quad \textit{for all} \quad \alpha \in \mathrm{I};$$

$$(21) \qquad f_{\alpha\beta}(\mathrm{A}_\beta) \subset \mathrm{A}_\alpha \quad \textit{whenever} \quad \alpha \leqslant \beta.$$

$\mathfrak{A} = (A_\alpha)$ と $\mathfrak{A}' = (A'_\alpha)$ が $\Sigma$ のいずれか 2 つの元である場合、関係 $\mathfrak{A} \leqslant \mathfrak{A}'$ はすべての $\alpha$ に対して $A_\alpha \supset A'_\alpha$ を意味します。明らかに、$\Sigma$ はこの関係によって *命令*されています。

(1) まず、順序付けられた集合 $\Sigma$ が *帰納的*であることを示しましょう。 L を完全に順序付けされた集合とし、$\lambda \to \mathfrak{A}^\lambda = (A^\lambda_\alpha)_{\alpha \in I}$ を L の $\Sigma$ への真に増加する写像とします。 $\alpha \in I$ ごとに、$B_\alpha = \bigcap_{\lambda \in L} A^\lambda_\alpha$ を入力します。次に、族 $\mathfrak{B} = (B_\alpha)_{\alpha \in I}$ が (21) を満たすことがすぐにわかります。 (i) と (ii) の理由により、(20) も満たすので、属するから $\Sigma$ になります。そして、$\mathfrak{B}$が$\mathfrak{A}^\lambda$の集合の上界であることは明らかです。

(2) $\mathfrak{A} = (A_\alpha)$ を $\Sigma$ の*最大値* 元とします。 $\alpha \leqslant \beta$ になるたびに $A_\alpha = f_{\alpha\beta}(A_\beta)$ であることを示します。すべての $\alpha \in I$ を $A'_\alpha = \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(A_\beta)$ とし、$\mathfrak{A}' = (A'_\alpha)$ 属するから $\Sigma$ までを示しましょう。 注意まず、$\alpha \leqslant \beta \leqslant \gamma$ の場合、(21) によって $f_{\alpha\gamma}(A_\gamma) = f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) \subset f_{\alpha\beta}(A_\beta)$ が得られます。さらに$f_{\alpha\beta}(A_\beta) \in \mathfrak{S}_\alpha$は(iv)で、$f_{\alpha\beta}(A_\beta) \neq \emptyset$は(20)で表されます。従って、条件 (i) と (ii) は、$\mathfrak{A}'$ が (20) を満たすことを示しています。また、$\alpha \leqslant \beta$ の場合、

$$f_{\alpha\beta}(A'_\beta) \subset \bigcap_{\gamma \geqslant \beta} f_{\alpha\beta}(f_{\beta\gamma}(A_\gamma)) = \bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma);$$

そして、それぞれの $\delta \geqslant \alpha$ には、$\gamma \geqslant \delta$ と $\gamma \geqslant \beta$ のような $\gamma \in I$ が存在し、その結果、$f_{\alpha\gamma}(A_\gamma) \subset f_{\alpha\delta}(A_\delta)$ となります。

$$\bigcap_{\gamma \geqslant \beta} f_{\alpha\gamma}(A_\gamma) = \bigcap_{\delta \geqslant \alpha} f_{\alpha\delta}(A_\delta) = A'_\alpha.$$

従って、$\mathfrak{A}'$ は (21) を満たし、したがって属するから $\Sigma$ になります。すべての $\alpha$ に対して $A'_\alpha \subset A_\alpha$ であるため、$\Sigma$ における $\mathfrak{A}$ の最大値は $\mathfrak{A}' = \mathfrak{A}$ を意味し、主張が証明されます。

(3) 次に、$\mathfrak{A} = (A_\alpha)$ が $\Sigma$ の *最大* 元である場合、$A_\alpha$ のそれぞれは *単一の元* から構成されることを確立します。 $x_\alpha \in A_\alpha$ にしましょう。それぞれの $\beta \geqslant \alpha$ に $B_\beta = A_\beta \cap \overset{-1}{f}_{\alpha\beta}(x_\alpha)$ を入力します。 $\beta$ が $\geqslant \alpha$ でない場合は、$B_\beta = A_\beta$ を入力します。次に、$\mathfrak{B} = (B_\beta)$ 属するから $\Sigma$ がわかります。 $\beta$ が $\geqslant \alpha$ ではない場合、関係 $\beta \leqslant \gamma$ は $f_{\beta\gamma}(B_\gamma) \subset f_{\beta\gamma}(A_\gamma) \subset A_\beta = B_\beta$ を意味します。一方、$\alpha \leqslant \beta \leqslant \gamma$ の場合は、

$$\overset{-1}{f}_{\alpha\gamma}(x_\alpha) = \overset{-1}{f}_{\beta\gamma}(\overset{-1}{f}_{\alpha\beta}(x_\alpha)),$$

我々は持っています

$$f_{\beta\gamma}(\overset{-1}{f}_{\alpha\gamma}(x_\alpha)) \subset \overset{-1}{f}_{\alpha\beta}(x_\alpha),$$

そして、$f_{\beta\gamma}(A_\gamma) \subset A_\beta$ から、再び $f_{\beta\gamma}(B_\gamma) \subset B_\beta$ が得られ、家族 $\mathfrak{B}$ は (21) を満たします。 証明の部分 (2) によって $\alpha \leqslant \beta$ になるたびに $A_\alpha = f_{\alpha\beta}(A_\beta)$ が発生するため、すべての $\beta \in \mathrm{I}$ に対して $\mathrm{B}_\beta \neq \emptyset$ であることは明らかです。最後に、(i) と (iii) のおかげで、すべての $\beta \in \mathrm{I}$ に対して $\mathrm{B}_\beta \in \mathfrak{S}_\beta$ が得られ、したがって $\mathfrak{B} \in \Sigma$ になります。すべての $\beta \in \mathrm{I}$ に対して $\mathrm{B}_\beta \subset \mathrm{A}_\beta$ であるため、$\mathfrak{A}$ の最大値は、すべての $\beta$、特に $\mathrm{A}_\alpha = \{x_\alpha\}$ に対して $\mathrm{B}_\beta = \mathrm{A}_\beta$ を意味します。

(4) 定理 1 を証明する立場になりました。(a) から始めましょう。我々は持っています

$$f_\alpha(\mathrm{E}) \subset \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta).$$

逆に、

$$x_\alpha \in \bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta),$$

そして置きます

$$\mathrm{B}_\beta = \overset{-1}{f}_{\alpha\beta}(x_\alpha)$$

$\beta \geqslant \alpha$ の場合、それ以外の場合は $\mathrm{B}_\beta = \mathrm{E}_\beta$ です。 $x_\alpha$の定義までに、$\mathrm{B}_\beta$は空ではなくなり、(iii)と(i)のおかげで、すべての$\beta \in \mathrm{I}$に対して$\mathrm{B}_\beta \in \mathfrak{S}_\beta$が得られます。さらに、$\beta \leqslant \gamma$ のときは常に $f_{\beta\gamma}(\mathrm{B}_\gamma) \subset \mathrm{B}_\beta$ であることは明らかです。したがって$\mathfrak{B} = (\mathrm{B}_\beta) \in \Sigma$です。 $\mathfrak{A} = (\mathrm{A}_\alpha)$ を $\Sigma$ の極大元とし、$\mathfrak{A} \geqslant \mathfrak{B}$ とします ($\mathfrak{A}$ の存在は (1) と §2, no. 4、定理 2、系 1 から得られます)。 (3) により、$\mathrm{A}_\beta$ はすべての $\beta \in \mathrm{I}$ に対して形 $\{y_\beta\}$ であるため、$y = (y_\beta)$ 属するは E となり、$f_\alpha(y) = y_\alpha = x_\alpha$ は定義となる。

最後に、(a) は (b) を意味します。 I は空ではないと仮定することもできます (そうでない場合、証明するものは何もありません)。 $\mathrm{E}_\alpha$ が空ではないという仮定は、すべての $\beta \geqslant \alpha$ に対して $f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$ であることを意味します。 $f_{\alpha\beta}(\mathrm{E}_\beta)$ なので、固定 $\alpha$ と変数 $\beta \geqslant \alpha$、形 $\mathrm{E}_\alpha$ 所属から $\mathfrak{S}_\alpha$ の部分集合の左有向集合は、条件 (ii)$'$ によって証明されます。

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset.$$

したがって、(a) により $f_\alpha(\mathrm{E}) \neq \emptyset$ となり、*なおさら* $\mathrm{E} \neq \emptyset$ となります。 Q.E.D.

#### 注意 {#ens-iii-s7-n4-rem-1 .statement tag=03OJ}

定理 1 の条件 (iii) が次のより弱い条件に置き換えられるとします。

(iii)$'$ *それぞれ* $\alpha \in \mathrm{I}$ *および空でないそれぞれの集合* $\mathrm{M}_\alpha \in \mathfrak{S}_\alpha$ *存在します* $x_\alpha \in \mathrm{M}_\alpha$ *そのような* $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ *それぞれ* $\beta \geqslant \alpha$。

この場合、定理 1 の結論 (b) は依然として有効です。 $\overset{-1}{f}_{\alpha\beta}(x_\alpha)$ がすべての $\beta \geqslant \alpha$ について $\mathfrak{S}_\beta$ に属するように $x_\alpha \in \mathrm{A}_\alpha$ を取ることに注意する限り、定理 1 の部分 (1) と (2) の証明は変更されず、部分 (3) の証明は有効のままです。 最後に、(4) の証明は、次のことを示します。

$$\bigcap_{\beta \geqslant \alpha} f_{\alpha\beta}(\mathrm{E}_\beta) \neq \emptyset$$

そして、このセットで $\beta \geqslant \alpha$ のときは常に $\overset{-1}{f}_{\alpha\beta}(x_\alpha) \in \mathfrak{S}_\beta$ となるように $x_\alpha$ を選択すると、 $f_\alpha(y) = x_\alpha$ となるような $y \in E$ が存在し、これが私たちの主張を証明します。

*例*

#### 例 1 {#ens-iii-s7-n4-exa-1 .statement tag=03TK}

$E_\alpha$ が *有限* 集合である場合、$\mathfrak{S}_\alpha$ を $E_\alpha$ の *すべて* 部分集合の集合とすることで、定理 1 を適用できます。 \* この例は、*一般位相* で、$E_\alpha$ が *コンパクト* トポロジー 空間、$f_{\alpha\beta}$ *連続* 写像、および $\mathfrak{S}_\alpha$ 集合の *閉じた* 部分集合である状況に一般化されます。 $E_\alpha$ (*一般位相*、章 I, § 9, no. 6)。 \*

#### 例 2 {#ens-iii-s7-n4-exa-2 .statement tag=03TL}

\* A を単位元とともに環とし、それぞれの $\alpha \in I$ について $T_\alpha$ を *アルティン* 左A-加群とします。 $E_\alpha$ を $T_\alpha$ に対して *同次の空間* とし、その上で $T_\alpha$ が忠実に動作するようにします (つまり、 $E_\alpha$ は $T_\alpha$ に接続された * アフィン空間* になります)。 $\beta \geqslant \alpha$ については、$f_{\alpha\beta} : E_\beta \to E_\alpha$ が *アフィン写像* であると仮定します。 $\mathfrak{S}_\alpha$ を、空の集合と $E_\alpha$ の *アフィン線形多様体* の集合からなるとします。この場合、条件 (i) は自明に満たされ、(ii) $T_\alpha$ はアルティンであるという事実から導かれます。なぜなら、これは、集合 $M \in \mathfrak{F}$ の有限共通部分の集合に極小元が存在し、この極小元が$\bigcap_{M \in \mathfrak{F}} M$ に等しくなければならないことを意味しているからです。最後に、$f_{\alpha\beta}$ はアフィンであるため、条件 (iii) と (iv) は自明に満たされます。 \*

### 5. 直接極限

I を (*正しい*) *有向* 事前注文された集合とし、$(E_\alpha)_{\alpha \in I}$ を I によってインデックス付けされた集合のファミリーとします。 $\alpha \leqslant \beta$ となるような対 $(\alpha, \beta)$ 、 元 、 I について、 $f_{\beta\alpha}$ を * $E_\alpha$ * $E_\beta$ の * 写像とします。 $f_{\beta\alpha}$ 満たすが次の条件であると仮定します。

(LI$_\mathrm{I}$) *関係* $\alpha \leqslant \beta \leqslant \gamma$ *暗示* $f_{\gamma\alpha} = f_{\gamma\beta} \circ f_{\beta\alpha}$。
(LI$_\mathrm{II}$) *それぞれ* $\alpha \in I, f_{\alpha\alpha}$ *は* $E_\alpha$の恒等写像です。

G を集合とします。これは、集合 $(E_\alpha)_{\alpha \in I}$ (章 II, § 4, no. 8) の族の *和* です。言葉の乱用により、G の標準像を含む $E_\alpha$ を同一視するとし、$x \in G$ ごとに$x \in E_\alpha$ となるような固有の添字 $\alpha \in I$ を $\lambda(x)$ で表すことにします。 G の 2 つの元 $x$, $y$ の間に次の関係を$R\{x, y\}$ で表すとします: 「$f_{\gamma\alpha}(x) = f_{\gamma\beta}(y)$ に対して $\gamma \geqslant \alpha = \lambda(x)$ と $\gamma \geqslant \beta = \lambda(y)$ となる元 $\gamma \in I$ が存在します。」この場合、R は * G 上の *同値関係です。R が再帰的であり、G 上で対称であることは明らかです。R が推移的であることを示すために、$x \in E_\alpha, y \in E_\beta, z \in E_\gamma$ とし、$\lambda \geqslant \alpha$、$\lambda \geqslant \beta$、$f_{\lambda\alpha}(x) = f_{\lambda\beta}(y)$ のような $\lambda \in I$ と、次のような $\mu \in I$ が存在すると仮定します。 $\mu \geqslant \beta$、$\mu \geqslant \gamma$、$f_{\mu\beta}(y) = f_{\mu\gamma}(z)$。 I は有向集合であるため、$\nu \geqslant \lambda$ と $\nu \geqslant \mu$ のような $\nu \in I$ が存在します。

$(\mathrm{LI_I})$までに

$$f_{\nu\alpha}(x) = f_{\nu\lambda}(f_{\lambda\alpha}(x)) = f_{\nu\lambda}(f_{\lambda\beta}(y)) = f_{\nu\beta}(y)$$
$$= f_{\nu\mu}(f_{\mu\beta}(y)) = f_{\nu\mu}(f_{\mu\gamma}(z)) = f_{\nu\gamma}(z),$$

それが私たちの主張を確立します。 商集合 $\mathrm{E} = \mathrm{G/R}$ は、写像* $(f_{\beta\alpha})$ の家族に関して、*家族* $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ の *直接の極限と呼ばれ、曖昧さの危険がない場合は $\mathrm{E} = \varinjlim (\mathrm{E}_\alpha, f_{\beta\alpha})$ または単に $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ と書かれます。言葉の乱用により、対 $((\mathrm{E}_\alpha), (f_{\beta\alpha}))$ (通常は $(\mathrm{E}_\alpha, f_{\beta\alpha})$ と表記されます) は、有向集合 I に対して、集合* の *直接系と呼ばれます。

¶ $\mathrm{E}_\alpha$ の少なくとも 1 つが空でない限り、明らかに E は空ではありません。 G の標準写像 $f$ から $\mathrm{E} = \mathrm{G/R}$ までを $f_\alpha$ 制限から $\mathrm{E}_\alpha$ で表します。 $f_\alpha$ は、$\mathrm{E}_\alpha$ の *標準写像* を E に変換したものと呼ばれます。$\alpha \leqslant \beta$ の場合、関係になります。

(22) $$f_\beta \circ f_{\beta\alpha} = f_\alpha$$

それぞれの $x \in \mathrm{E}_\alpha$ には $(\mathrm{LI_I})$ による $f_{\beta\beta}(f_{\beta\alpha}(x)) = f_{\beta\alpha}(x)$ があるためです。したがって、元 $x \in \mathrm{E}_\alpha$ と $f_{\beta\alpha}(x) \in \mathrm{E}_\beta$ は合同 mod R です。

*例*

#### 例 1 {#ens-iii-s7-n5-exa-1 .statement tag=03TM}

A、B を 2 つの集合とし、$(\mathrm{V}_\alpha)_{\alpha \in \mathrm{I}}$ を A の部分集合の家族とし、その添字集合 I が方向付けられ、関係 $\alpha \leqslant \beta$ が $\mathrm{V}_\beta \subset \mathrm{V}_\alpha$ を暗示するようにします。 $\mathrm{E}_\alpha$ は、$\mathrm{V}_\alpha$ のすべての写像の集合を B に表し、添字 $(\alpha, \beta)$ の各対について、$\alpha \leqslant \beta$ は $f_{\beta\alpha}$ が $\mathrm{E}_\alpha$ の写像になるようにします。 $\mathrm{E}_\beta$ は、各写像 $u \in \mathrm{E}_\alpha$ を *制限* から $\mathrm{V}_\beta$ に送信します。 条件 $(\mathrm{LI_I})$ と $(\mathrm{LI_{II}})$ が満たされることは明らかで、$\mathrm{V}_\alpha$ の写像* の * 細菌の集合 $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ が B に集合と呼ばれます。 \* 最も頻繁に発生するケースは、$(\mathrm{V}_\alpha)$ が次の家族である場合です。トポロジカル空間 A の部分集合の *近傍* (*一般位相*、章 I, §6, no. 10)。 \*

#### 例 2 {#ens-iii-s7-n5-exa-2 .statement tag=03TN}

それぞれの $\alpha \in \mathrm{I}$ について、$\mathrm{E}_\alpha$ は同じ集合 F であり、$\alpha \leqslant \beta$、$f_{\beta\alpha}$ はそれ自体に対する F の恒等写像であるとします。次に、F 上に $\varinjlim \mathrm{E}_\alpha$ の *標準全単射* が存在します。順序から定義する $\varinjlim \mathrm{E}_\alpha$ では、$(\mathrm{E}_\alpha)$ 族の和である形集合 G でなければなりません。したがって、G は相互に互いに素集合の家族 $(\mathrm{G}_\alpha)$ の和集合であり、それぞれの $\alpha \in \mathrm{I}$ に対して正規の全単射 $h_\alpha : \mathrm{F} \to \mathrm{G}_\alpha$ が存在します。次に、G 上の同値関係 R 対応するから分割 $(\mathrm{P}_y)_{y \in \mathrm{F}}$ を考慮する必要があります。ここで、$\alpha$ は I を通過するため、$\mathrm{P}_y$ はすべての $h_\alpha(y)$ の集合です。明らかに、$y \to \mathrm{P}_y$ は全単射であり、その逆数は全単射である必要があります。この標準的な全単射を使用して、$\varinjlim \mathrm{E}_\alpha$ と同一視する F を実行します。

#### 補題 1 {#ens-iii-s7-lem-1 .statement tag=03OK}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$ *を集合の直接系とし、* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *その直接の極限とし、それぞれ* $\alpha \in \mathrm{I}$ *$f_\alpha \colon \mathrm{E}_\alpha \to \mathrm{E}$ *標準写像とします。*

(i) *$(x^{(i)})_{1 \leqslant i \leqslant n}$ を * E の元の有限系とします。 *すると、* $\alpha \in I$ * そして有限系* $(x_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *of 元 of* $E_\alpha$ *そのような* $x^{(i)} = f_\alpha(x_\alpha^{(i)})$ *$1 \leqslant i \leqslant n$ 用。

(ii) *$(y_\alpha^{(i)})_{1 \leqslant i \leqslant n}$ *をある * $E_\alpha$ の元の有限系とする。 *もし* $f_\alpha(y_\alpha^{(i)}) = f_\alpha(y_\alpha^{(j)})$ *各対の添字* $(i, j)$ に対して、 *$\beta \geqslant \alpha$ *そのような* $f_{\beta\alpha}(y_\alpha^{(i)}) = f_{\beta\alpha}(y_\alpha^{(j)})$ *各対* $(i, j)$ が存在します。

(i) E の定義により、$i$ 添字 $\beta_i \in I$ および元 $z_{\beta_i} \in E_{\beta_i}$ に対して $x^{(i)} = f_{\beta_i}(z_{\beta_i})$ が存在します。 $\alpha$ を、$\alpha \geqslant \beta_i$ が $1 \leqslant i \leqslant n$ となり、$x_\alpha^{(i)} = f_{\alpha\beta_i}(z_{\beta_i})$ となるようにします。

(ii) E の定義により、対 $(i, j)$ ごとに、$\gamma_{ij} \geqslant \alpha$ と $f_{\gamma_{ij}\alpha}(y_\alpha^{(i)}) = f_{\gamma_{ij}\alpha}(y_\alpha^{(j)})$ となる$\gamma_{ij} \in I$ が存在します。すべての対 $(i, j)$ に対して $\beta \geqslant \gamma_{ij}$ となるように $\beta$ を取り、関係 $f_{\beta\alpha} = f_{\beta\gamma_{ij}} \circ f_{\gamma_{ij}\alpha}$ を使用します。

### 6. 直接系/写像

#### 命題 6 {#ens-iii-s7-prop-6 .statement tag=03RR}

*I *を有向集合とし、* $(E_\alpha, f_{\beta\alpha})$ *集合の直接系をIと相対させ、*$E = \varinjlim E_\alpha$を*直接の極限とし、それぞれ* $\alpha \in I$ *としましょう*

$$f_\alpha : E_\alpha \to E$$

*標準写像になります。それぞれ* $\alpha \in I$ に対して、* $u_\alpha$ * $E_\alpha$ の写像を * 集合* F * にします*

(23) $$u_\beta \circ f_{\beta\alpha} = u_\alpha \qquad \textit{whenever } \alpha \leqslant \beta.$$

*その後:*

(a) **E の *F に一意な写像* $u$ が存在します *そのような*

(24) $$u_\alpha = u \circ f_\alpha \qquad \textit{for all } \alpha \in I.$$

(b) $u$ *は、F *が集合* $u_\alpha(E_\alpha)$ の和集合である場合にのみ全射法です。

(c) $u$ *それぞれ* $\alpha \in I$ *関係* $x \in E_\alpha$、$y \in E_\alpha$、$u_\alpha(x) = u_\alpha(y)$ *$\beta \geqslant \alpha$ *そのような* $f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ が存在することを暗示します。

(a) no. 5の記法で、各$\alpha \in I$(章II, § 4, no. 7、命題8)の$E_\alpha$の$u_\alpha$と一致するGの写像をFに$v$とします。 仮定は、$v$ が同値関係 R (章 II, § 6, no. 5) と互換性があることを意味します。したがって、F には $v = u \circ f$ となる $E = G/R$ の一意な写像 $u$ が存在します (*loc. cit.*)。

(b) E は $f_\alpha(E_\alpha)$ の和集合であるため、関係 $F = \bigcup_{\alpha \in I} u_\alpha(E_\alpha)$ は明らかに $u$ が全射であるために必要かつ十分です。

(c) no. 5 の補題 1 により、$\mathbf{E}$ の任意の 2 つの元は常に形 $f_\alpha(x)$ と $f_\alpha(y)$ に書き込むことができます。ここで、$x \in \mathrm{E}_\alpha$ と $y \in \mathrm{E}_\alpha$ は、適切な選択に対応します。 $\alpha \in \mathrm{I}$。 補題から、関係 $f_\alpha(x) = f_\alpha(y)$ は、$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ のような $\beta \geqslant \alpha$ の存在と同等であることがわかります。 $u_\alpha(x) = u(f_\alpha(x))$と$u_\alpha(y) = u(f_\alpha(y))$なので、これで証明が完成します。

¶ 写像 $u$ が*全単射*である場合、言葉の乱用により、ときどきは F が家族 $(\mathrm{E}_\alpha)$ の直接の極限であると言われます。

#### 注意 {#ens-iii-s7-n6-rem-1 .statement tag=03OL}

写像 $f_{\beta\alpha}$ がそれぞれ*単射*であると仮定します。次に、それぞれの $f_\alpha$ は、関係 R の定義によって *単射的* です。この場合、一般的に同一視する $\mathrm{E}_\alpha$ と $f_\alpha(\mathrm{E}_\alpha)$ であり、したがって E を $\mathrm{E}_\alpha$ の *和集合* とみなします。逆に、$(\mathrm{F}_\alpha)_{\alpha \in \mathrm{I}}$ を集合 F の部分集合の増加するファミリーとし、F をこのファミリーの *和集合* と仮定します。 $j_{\beta\alpha}$ が $\alpha \leqslant \beta$ の $\mathrm{F}_\beta$ への $\mathrm{F}_\alpha$ の標準単射を表す場合、命題 6 から、写像の家族に関して、家族 $\mathrm{F}_\alpha$ の直接の極限と同一視する F が得られることがわかります。 $(j_{\beta\alpha})$、および$\mathrm{F}_\alpha$の標準写像を$\varinjlim \mathrm{F}_\alpha$に、$\mathrm{F}_\alpha$の標準単射をFに、それぞれ$\alpha \in \mathrm{I}$に。

#### 系 1 {#ens-iii-s7-prop-6-cor-1 .statement tag=03RS}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$ *と* $(\mathrm{F}_\alpha, g_{\beta\alpha})$ *を、同じ添字集合* I に対する集合の 2 つの直接系とします。 *let* $\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{F} = \varinjlim \mathrm{F}_\alpha$、*そしてそれぞれ* $\alpha \in \mathrm{I}$ *let* $f_\alpha$ (*resp.* $g_\alpha$) *標準写像 of* $\mathrm{E}_\alpha$ (*resp.* $\mathrm{F}_\alpha$) *into* E (*resp.* F)。 *それぞれ* $\alpha \in \mathrm{I}$ *させて* $u_\alpha$ *$\mathrm{E}_\alpha$の写像を*に* $\mathrm{F}_\alpha$ *いつでも* $\alpha \leqslant \beta$, *図式*

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_{\beta\alpha}}\big\downarrow & & \big\downarrow{\scriptstyle g_{\beta\alpha}} \\ \mathrm{E}_\beta & \underset{u_\beta}{\longrightarrow} & \mathrm{F}_\beta \end{array}$$

*は可換です。次に、 一意な写像* $u : \mathrm{E} \rightarrow \mathrm{F}$ *それぞれについて* $\alpha \in \mathrm{I}$、*図式* が存在します。

$$\begin{array}{ccc} \mathrm{E}_\alpha & \overset{u_\alpha}{\longrightarrow} & \mathrm{F}_\alpha \\ {\scriptstyle f_\alpha}\big\downarrow & & \big\downarrow{\scriptstyle g_\alpha} \\ \mathrm{E} & \underset{u}{\longrightarrow} & \mathrm{F} \end{array}$$

*は可換です。*

$v_\alpha = g_\alpha \circ u_\alpha$を入れます。 $\alpha \leqslant \beta$ の場合、(22) までに次のようになります。

$$v_\beta \circ f_{\beta\alpha} = g_\beta \circ u_\beta \circ f_{\beta\alpha} = g_\beta \circ g_{\beta\alpha} \circ u_\alpha = g_\alpha \circ u_\alpha = v_\alpha.$$

したがって、命題を適用する 6 から写像 $v_\alpha$、よっての存在と写像 $u : \mathrm{E} \to \mathrm{F}$ の一意性は次のようになります。

$$u \circ f_\alpha = v_\alpha = g_\alpha \circ u_\alpha$$

すべての$\alpha \in \mathrm{I}$に。

¶ 系 1 の条件を満たす写像 $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$ の族は、$(\mathrm{E}_\alpha, f_{\beta\alpha})$ の写像* から $(\mathrm{F}_\alpha, g_{\beta\alpha})$ への *直接系と呼ばれます。 系 1 で定義された写像は、ファミリー $(u_\alpha)$ の *直接極限* と呼ばれ、曖昧さの危険がない場合は $u = \varinjlim u_\alpha$ と書かれます。

#### 系 2 {#ens-iii-s7-prop-6-cor-2 .statement tag=03RT}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$、$(\mathrm{F}_\alpha, g_{\beta\alpha})$、$(\mathrm{G}_\alpha, h_{\beta\alpha})$ *Iに対する集合の3つの直接系とします。 *$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{F} = \varinjlim \mathrm{F}_\alpha$、$\mathrm{G} = \varinjlim \mathrm{G}_\alpha$、*そして* $f_\alpha$ *(それぞれ* $g_\alpha$、$h_\alpha$*) を* $\mathrm{E}_\alpha$ *(それぞれ* $\mathrm{F}_\alpha$、$\mathrm{G}_\alpha$*) の標準写像とします* E *(それぞれ* F、G*)。 * $(u_\alpha)$ * と* $(v_\alpha)$ * が 2 つの直接系の写像* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$、$v_\alpha : \mathrm{F}_\alpha \to \mathrm{G}_\alpha$ の場合、*その後写像* $v_\alpha \circ u_\alpha : \mathrm{E}_\alpha \to \mathrm{G}_\alpha$ * 形直接系の写像、そして私たちは*

(25) $$\varinjlim (v_\alpha \circ u_\alpha) = (\varinjlim v_\alpha) \circ (\varinjlim u_\alpha).$$

$w_\alpha = v_\alpha \circ u_\alpha$ とすると、$\alpha \leqslant \beta$ は次のようになります。

$$h_{\beta\alpha} \circ w_\alpha = (h_{\beta\alpha} \circ v_\alpha) \circ u_\alpha = (v_\beta \circ g_{\beta\alpha}) \circ u_\alpha = v_\beta \circ (u_\beta \circ f_{\beta\alpha}) = w_\beta \circ f_{\beta\alpha},$$

これは、$(w_\alpha)$ が写像の直接系であることを示しています。さらに、$u = \varinjlim u_\alpha$ と $v = \varinjlim v_\alpha$ の場合、すべての $\alpha \in \mathrm{I}$ について、

$$(v \circ u) \circ f_\alpha = v \circ (g_\alpha \circ u_\alpha) = h_\alpha \circ (v_\alpha \circ u_\alpha),$$

そして直接極限の一意性のおかげで、$v \circ u = \varinjlim w_\alpha$が得られます。

#### 命題 7 {#ens-iii-s7-prop-7 .statement tag=03RU}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$ *と* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *を* Iに対する集合の2つの直接系とし、*それぞれ* $\alpha \in \mathrm{I}$ *$u_\alpha$ *を* $\mathrm{E}_\alpha$の写像 *にします* $\mathrm{E}'_\alpha$ *そのような* $u_\alpha$ *形直接系の写像。しましょう* $u = \varinjlim u_\alpha$。 *それぞれ* $u_\alpha$ *が単射* (または *全射*) の場合*、* $u$ *は単射* (*全射*) です。

$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$、$f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$、$f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$を標準写像とします。それぞれの $u_\alpha$ が単射であると仮定します。 $u$ が単射であることを示すには、命題 6 によって、$x \in \mathrm{E}_\alpha$ と $y \in \mathrm{E}_\alpha$ が $f'_\alpha(u_\alpha(x)) = f'_\alpha(u_\alpha(y))$ となる場合、$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ となる$\beta \geqslant \alpha$ が存在することを検証するだけで十分です。ここで、仮定は、(no. 6, 補題 1) という$\beta \geqslant \alpha$ が存在することを意味します。

$$f'_{\beta\alpha}(u_\alpha(x)) = f'_{\beta\alpha}(u_\alpha(y)), \qquad \text{i.e.,} \qquad u_\beta(f_{\beta\alpha}(x)) = u_\beta(f_{\beta\alpha}(y)),$$

したがって、$u_\beta$ は単射法であるため、$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$ となります。

ここで、$u_\alpha$ が全射であると仮定します。それでは、

$$\mathrm{E}' = \bigcup_\alpha f'_\alpha(\mathrm{E}'_\alpha) = \bigcup_\alpha f'_\alpha(u_\alpha(\mathrm{E}_\alpha)) = \bigcup_\alpha u(f_\alpha(\mathrm{E}_\alpha)) = u\Big(\bigcup_\alpha f_\alpha(\mathrm{E}_\alpha)\Big) = u(\mathrm{E}).$$

命題 7 の記法では、$\alpha \in \mathrm{I}$ ごとに $\mathrm{M}_\alpha$ を $\mathrm{E}_\alpha$ の部分集合とします。 $\alpha \leqslant \beta$ のときはいつでも $f_{\beta\alpha}(\mathrm{M}_\alpha) \in \mathrm{M}_\beta$ がある場合、家族 $(\mathrm{M}_\alpha)_{\alpha \in \mathrm{I}}$ は * $\mathrm{E}_\alpha$ の部分集合の *直接系であると言われます。 $g_{\beta\alpha}$ ($\alpha \leqslant \beta$) を $\mathrm{M}_\alpha$ から $\mathrm{M}_\beta$ までの写像とします。そのグラフは、$f_{\beta\alpha}$ から $\mathrm{M}_\alpha$ の制限のグラフと同じです。すると、$(\mathrm{M}_\alpha, g_{\beta\alpha})$ が集合の直接系であることは明らかです。そして、命題 7 を標準単射 $j_\alpha : \mathrm{M}_\alpha \to \mathrm{E}_\alpha$ に適用すると、単射 $j = \varinjlim j_\alpha$ によって E の部分集合を使用して *同一視する* $\mathrm{M} = \varinjlim \mathrm{M}_\alpha$ が可能になります。

#### 系 {#ens-iii-s7-n6-cor-1 .statement tag=03ON}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$ *と* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ *を集合の2つの直接系とし、* $(u_\alpha)$ *を写像* $u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'_\alpha$の直接系とし、*そして* $u = \varinjlim u_\alpha$とします。

(i) *$(\mathrm{M}_\alpha)$ *を * $\mathrm{E}_\alpha$ の部分集合の直接系とします。 *すると* $(u_\alpha(\mathrm{M}_\alpha))$ *は* $\mathrm{E}'_\alpha$の部分集合の直接系です、*そして私たちは*

(26) $$\varinjlim u_\alpha(\mathrm{M}_\alpha) = u\,(\varinjlim \mathrm{M}_\alpha).$$

(ii) *$(a'_\alpha)_{\alpha \in \mathbf{I}}$ *そのような家族にしましょう* $a'_\alpha \in \mathrm{E}'_\alpha$ *それぞれに* $\alpha \in \mathrm{I}$ *そして* $f'_{\beta\alpha}(a'_\alpha) = a'_\beta$ *いつでも* $\alpha \leqslant \beta$。 *次に集合* $\overset{-1}{u}_\alpha(a'_\alpha)$ *形直接系の部分集合の * $\mathrm{E}_\alpha$、 *そして我々は*

(27) $$\varinjlim \overset{-1}{u}_\alpha(a'_\alpha) = \overset{-1}{u}(a'),$$

*ここで* $a'$ *は* $\varinjlim \mathrm{E}'_\alpha$の一意元です *これは* $a'_\alpha$ *それぞれ* $\alpha \in \mathrm{I}$の標準像です。

(i) $\mathrm{E}'_\alpha$ の部分集合の $u_\alpha(\mathrm{M}_\alpha)$ 形直接系は明らかであり、$v_\alpha$ が $\mathrm{M}_\alpha$ の写像である$u_\alpha(\mathrm{M}_\alpha) = v_\alpha(\mathrm{M}_\alpha)$ を同じグラフである $u_\alpha(\mathrm{M}_\alpha)$ に書き込むことができます。 $u_\alpha$から$\mathrm{M}_\alpha$の制限のものとして。 $v_\alpha$ は全射なので、公式 (26) は命題 7 から続きます。

(ii) $\mathrm{N}_\alpha = \overset{-1}{u}_\alpha(a'_\alpha)$ とします。 $\alpha \leqslant \beta$ と $x_\alpha \in \mathrm{N}_\alpha$ の場合、

$$u_\beta(f_{\beta\alpha}(x_\alpha)) = f'_{\beta\alpha}(u_\alpha(x_\alpha) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta;$$

従って $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$、そして $\mathrm{N}_\alpha$ 従って、$\mathrm{E}_\alpha$ の部分集合の形直接系です。 命題 7 の証明の記法では、元 $x \in \varinjlim \mathrm{N}_\alpha$ を検討します。 $x = f_\alpha(x_\alpha)$ となるような $\alpha \in \mathrm{I}$ と $x_\alpha \in \mathrm{N}_\alpha$ が存在するため、$u(x) = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha) = a'$ となります。逆に、一部の $\alpha \in \mathrm{I}$ と一部の $x_\alpha \in \mathrm{E}_\alpha$ が $x \in \overset{-1}{u}(a')$ で、$x = f_\alpha(x_\alpha)$ であれば、$a' = u(f_\alpha(x_\alpha)) = f'_\alpha(u_\alpha(x_\alpha)) = f'_\alpha(a'_\alpha)$ になります。従って (no. 5, 補題 1) $f'_{\beta\alpha}(u'_\alpha(x_\alpha)) = f'_{\beta\alpha}(a'_\alpha) = a'_\beta$ となるような $\beta \geqslant \alpha$ が存在します。つまり、$u_\alpha(f_{\beta\alpha}(x_\alpha)) = a'_\beta$、つまり $f_{\beta\alpha}(x_\alpha) \in \mathrm{N}_\beta$ です。 $x = f_\beta(f_{\beta\alpha}(x_\alpha))$ なので、$x \in \varinjlim \mathrm{N}_\alpha$ になります。

#### 注意 {#ens-iii-s7-n6-rem-2 .statement tag=03OO}

各 $\alpha \in \mathrm{I}$ について、$u_\alpha : \mathrm{E}_\alpha \to \mathrm{E}'$ が写像であり、族 $(u_\alpha)$ が (23) を満たすとします。 I に対する直接系 $(\mathrm{E}_\alpha, i_{\beta\alpha})$ を考えます。ここで、$\mathrm{E}'_\alpha = \mathrm{E}'$ はすべての $\alpha \in \mathrm{I}$ に対して、$i_{\beta\alpha}$ は $\mathrm{E}'$ の恒等写像です。この場合、(no. 5, 例 2) $\mathrm{E}'$ は正規的に $\varinjlim \mathrm{E}'_\alpha$ と識別できます。 $u_\alpha$ を $\mathrm{E}_\alpha$ の写像から $\mathrm{E}'_\alpha$ にすると考えると、$(u_\alpha)$ は写像の直接系となり、(24) で定義される写像 $u : \mathrm{E} \to \mathrm{E}'$ は、この直接の極限と同一視されます。 写像の系。従って、言葉の乱用により、$u = \varinjlim u_\alpha$と書きます。

J が (誘導された事前順序付けに関して) 指示された I の部分集合である場合、サブファミリー $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$ およびファミリー $(f_{\beta\alpha})$ の対からなるであることは明らかです。ここで、$\alpha \leqslant \beta$ と $\alpha \in \mathrm{J}$ および $\beta \in \mathrm{J}$、 J に対する集合の直接系です。それは、添字集合を J に*制限*することによって得られると言われています。 E、E' がそれぞれ家族 $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{I}}$ と $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}}$ の直接の極限を表し、それぞれの $\alpha \in \mathrm{I}$ について $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}$ が標準写像を表すものとします。次に、$(f_\alpha)_{\alpha \in \mathrm{J}}$ は写像の直接系であり、その結果、$g = \varinjlim f_\alpha$ は E' の E への写像であり、*標準* と呼ばれます。さらに、J' が J の有向部分集合であり、E'' が族 $(\mathrm{E}_\alpha)_{\alpha \in \mathrm{J}'}$ の直接極限であり、

$$g' : \quad \mathrm{E}'' \to \mathrm{E}' \qquad \text{and} \qquad g'' : \mathrm{E}'' \to \mathrm{E}$$

が標準写像である場合、命題 6 から次のことがすぐに続きます。

(28) $$g'' = g \circ g'.$$

#### 命題 8 {#ens-iii-s7-prop-8 .statement tag=03OP}

*I *を有向集合とし、* $(\mathrm{E}_\alpha, f_{\beta\alpha})$ *をIを基準とした集合の直接系とし、*$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$ *を直接の極限とします。 * J * を * I * の余終値部分集合とし、* E' * $(\mathrm{E}_\alpha, f_{\beta\alpha})$ から * 添字集合を * J に制限することによって得られた集合の直接系の直接極限とする。 標準写像* $g$ *of* E' *into* E *は全単射です*。

J は必然的に有向集合 (§ 1, no. 10) になります。 命題 6 の基準を使用して、$g$ が全単射であることを示します。単射性の条件は、定義のすぐ後に続き、補題 1 の no. 5 から続きます。 $g$ が全射であることを示すために、各 $\alpha \in \mathrm{J}$ について、

$$g(\mathrm{E}_\alpha) = f_\alpha(\mathrm{E}_\alpha).$$

さて、それぞれの $\beta \in I$ に対して、$\beta \leqslant \gamma$ となるような $\gamma \in J$ が存在し、そこから $g(E_\gamma) \supset g(f_{\gamma\beta}(E_\beta)) = f_\beta(E_\beta)$ が導き出されます。したがって、$\alpha$ が J を通るので、E は集合 $g(E_\alpha)$ の和集合になります。

### 7. ダブルダイレクト極限。直接極限の積

I、L を 2 つの有向集合とし、$I \times L$ をその積 (§ 1, no. 4) とします。これは、積の予約注文により、再び有向集合になります。 $I \times L$ に対する集合 $(E^\lambda_\alpha, f^{\mu\lambda}_{\beta\alpha})$ の直接系を考えてみましょう。それから私たちは

$$(29) \qquad f^{\nu\lambda}_{\gamma\alpha} = f^{\mu\nu}_{\gamma\beta} \circ f^{\mu\lambda}_{\beta\alpha}$$

$\alpha \leqslant \beta \leqslant \gamma$ と $\lambda \leqslant \mu \leqslant \nu$ のたびに。

E または $\varinjlim_{\alpha,\lambda} E^\lambda_\alpha$ がこの直接系の直接の極限を表すものとします。それぞれの $\lambda \in L$ に $g^\lambda_{\beta\alpha} = f^{\lambda\lambda}_{\beta\alpha} : E^\lambda_\alpha \to E^\lambda_\beta$ を入れます。次に、(29) から次のようになります。

$$(30) \qquad g^\lambda_{\gamma\alpha} = g^\lambda_{\gamma\beta} \circ g^\lambda_{\beta\alpha} \qquad \text{whenever } \alpha \leqslant \beta \leqslant \gamma;$$

他の語では、$(E^\lambda_\alpha, g^\lambda_{\beta\alpha})$ は I に対して集合の直接系です。 $F^\lambda = \varinjlim_\alpha E^\lambda_\alpha$ をその直接の極限とします。 $\lambda \leqslant \mu$ が L の元に固定されている場合、(29) から、写像の写像 $h^{\mu\lambda}_\alpha = f^{\lambda\mu}_{\alpha\alpha} : E^\lambda_\alpha \to E^\mu_\alpha$ 形直接系となります。この系の写像の直接の極限を$h^{\mu\lambda} = \varinjlim_\alpha h^{\mu\lambda}_\alpha : F^\lambda \to F^\mu$とします。 L で $\lambda \leqslant \mu \leqslant \nu$ の場合、

$$(31) \qquad h^{\nu\lambda} = h^{\nu\mu} \circ h^{\mu\lambda}$$

(no. 6, 命題 6, 系 2) したがって、$(F^\lambda, h^{\mu\lambda})$ は、L に対して集合の直接系です。 $F = \varinjlim F^\lambda$ をその直接の極限とします。 定義するを *正規の全単射* $E \to F$ とします。この目的のために、$g^\lambda_\alpha$ は標準写像 $E^\lambda_\alpha \to F^\lambda$ と $h^\lambda$ 標準写像 $F^\lambda \to F$ を表し、$u^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha$ を置きます。 $\alpha \leqslant \beta$ と $\lambda \leqslant \mu$ の場合、次のようになります。

$$\begin{aligned} u^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} &= h^\mu \circ g^\mu_\beta \circ f^{\mu\lambda}_{\beta\alpha} = h^\mu \circ g^\mu_\beta \circ f^{\mu\mu}_{\beta\alpha} \circ f^{\mu\lambda}_{\alpha\alpha} = h^\mu \circ g^\mu_\alpha \circ f^{\mu\lambda}_{\alpha\alpha} \\ &= h^\mu \circ h^{\mu\lambda} \circ g^\lambda_\alpha = h^\lambda \circ g^\lambda_\alpha = u^\lambda_\alpha \end{aligned}$$

$h^{\mu\lambda}$の(29)と定義から。したがって、$I \times L$ に対する写像の $u^\lambda_\alpha$ 形直接系となります。 $u = \varinjlim_{\alpha,\lambda} u^\lambda_\alpha : E \to F$を入れます。 $u$ は no. 6, 命題 6 の基準適用により全単射であることを示します。そもそも、F は集合 $h^\lambda(F^\lambda)$ の和集合であり、それぞれの $F^\lambda$ は和集合です集合 $g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)$;したがって、F は集合の和集合です

$$h^\lambda(g_\alpha^\lambda(\mathrm{E}_\alpha^\lambda)) = u_\alpha^\lambda(\mathrm{E}_\alpha^\lambda).$$

次に、$x$、$y$を$\mathrm{E}_\alpha^\lambda$の2つの元とし、$u_\alpha^\lambda(x) = u_\alpha^\lambda(y)$、つまり$h^\lambda(g_\alpha^\lambda(x)) = h^\lambda(g_\alpha^\lambda(y))$とします。次に (no. 5, 補題 1) $h^{\mu\lambda}(g_\alpha^\lambda(x)) = h^{\mu\lambda}(g_\alpha^\lambda(y))$、つまり $g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_\alpha^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$ となるような $\mu \geqslant \lambda$ が存在します。同様に、$g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(x)) = g_{\beta\alpha}^\mu(f_{\alpha\alpha}^{\mu\lambda}(y))$ (no. 5, 補題 1) となるような$\beta \geqslant \alpha$、つまり $f_{\beta\alpha}^{\mu\lambda}(x) = f_{\beta\alpha}^{\mu\lambda}(y)$ が存在します。これは (no. 6, 命題 6) $u$ が単射であることを示しています。したがって、次のことを証明しました。

#### 命題 9 {#ens-iii-s7-prop-9 .statement tag=03RV}

*もし* $(\mathrm{E}_\alpha^\lambda, f_{\beta\alpha}^{\mu\lambda})$ * が積* $\mathrm{I} \times \mathrm{L}$ *2 つの有向集合に対して相対的に集合の直接系である場合、(正規の全単射まで)*

(32)
$$\varinjlim_{\alpha,\ \lambda} \mathrm{E}_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} \mathrm{E}_\alpha^\lambda).$$

#### 系 {#ens-iii-s7-n7-cor-1 .statement tag=03OQ}

*$(\mathrm{{E}'}^\lambda_\alpha, {f'}^{\mu\lambda}_{\beta\alpha})$ *を $\mathrm{I} \times \mathrm{L}$ に対して相対的に集合の他の直接系とし、*それぞれ* $(\alpha, \lambda) \in \mathrm{I} \times \mathrm{L}$ *$u_\alpha^\lambda$ *を* $\mathrm{E}_\alpha^\lambda$ *を* $\mathrm{{E}'}^\lambda_\alpha$ の写像として、 *次のように* $u_\alpha^\lambda$ *形直接系/写像。それでは*

(33)
$$\varinjlim_{\alpha,\ \lambda} u_\alpha^\lambda = \varinjlim_{\lambda}\ (\varinjlim_{\alpha} u_\alpha^\lambda).$$

検証は読者に任せます。

#### 命題 10 {#ens-iii-s7-prop-10 .statement tag=03RW}

*$(\mathrm{E}_\alpha, f_{\beta\alpha})$ * と* $(\mathrm{E}'_\alpha, f'_{\beta\alpha})$ * を集合の 2 つの直接系とし、どちらも同じ有向集合* I を基準にします。 *$\mathrm{E} = \varinjlim \mathrm{E}_\alpha$、$\mathrm{E}' = \varinjlim \mathrm{E}'_\alpha$、*そして* $f_\alpha : \mathrm{E}_\alpha \to \mathrm{E}, f'_\alpha : \mathrm{E}'_\alpha \to \mathrm{E}'$ *それぞれを* $\alpha \in \mathrm{I}$として、標準写像とします。 *すると* $(\mathrm{E}_\alpha \times \mathrm{E}'_\alpha, f_{\beta\alpha} \times f'_{\beta\alpha})$ *は集合の直接系、* $(f_\alpha \times f'_\alpha)$ *は写像の直接系、そして* $\varinjlim (f_\alpha \times f'_\alpha)$ *は全単射*

(34)
$$\varinjlim (\mathrm{E}_\alpha \times \mathrm{E}'_\alpha) \to (\varinjlim \mathrm{E}_\alpha) \times (\varinjlim \mathrm{E}'_\alpha).$$

命題の最初の 2 つの主張はすぐに検証されます。 $g = \varinjlim (f_\alpha \times f'_\alpha)$ が全単射であることを示すために、no. 6 の 6 を命題を適用するとします。明らかに、$\mathrm{E} \times \mathrm{E}'$ は集合 $f_\alpha(\mathrm{E}_\alpha) \times f'_\alpha(\mathrm{E}'_\alpha)$ の和集合です。したがって、$g$ は全射法です。 $(x, x')$ と $(y, y')$ が $f_\alpha(x) = f_\alpha(y)$ と $f'_\alpha(x') = f'_\alpha(y')$ となるような 2 つの $\mathrm{E}_\alpha \times \mathrm{E}'_\alpha$ の元である場合、(no. 5, 補題 1) の 2 つの元 $\beta$, $\gamma$ が存在します。 I は、$\beta \geqslant \alpha$、$\gamma \geqslant \alpha$、$f_{\beta\alpha}(x) = f_{\beta\alpha}(y)$、$f'_{\gamma\alpha}(x') = f'_{\gamma\alpha}(y')$ などです。 I が指示されているため、$\delta \geqslant \beta$ と $\delta \geqslant \gamma$ のような $\delta \in \mathrm{I}$ が存在します。したがって、$f_{\delta\alpha}(x) = f_{\delta\alpha}(y)$ と $f'_{\delta\alpha}(x') = f'_{\delta\alpha}(y')$ です。これで証明は完了です。

全単射 $g$ は *正規* と呼ばれます。

#### 系 {#ens-iii-s7-n7-cor-2 .statement tag=03RX}

*$(\mathrm{F}_\alpha, g_{\beta\alpha})$ *と* $(\mathrm{F}'_\alpha, g'_{\beta\alpha})$ *を* Iに対する集合の2つの直接系とし、*それぞれ* $\alpha \in \mathrm{I}$ *$u_\alpha : \mathrm{E}_\alpha \to \mathrm{F}_\alpha$、$u'_\alpha : \mathrm{E}'_\alpha \to \mathrm{F}'_\alpha$ *次のような写像とする* $(u_\alpha)$ *and* $(u'_\alpha)$ *は写像の 2 つの直接系です。すると* $(u_\alpha \times u'_\alpha)$ * は写像の直接系であり、(正規の全単射まで) *

(35) $$\varinjlim (u_\alpha \times u'_\alpha) = (\varinjlim u_\alpha) \times (\varinjlim u'_\alpha).$$

検証は読者に任せます。

### 練習問題 {#ens-iii-s7-exercises}

[§ 7 に対して練習問題](exercises/s7/)を参照してください。

[^1]: This means that $u_\alpha \circ f_{\alpha\beta} = g_{\alpha\beta} \circ u_\beta$.
