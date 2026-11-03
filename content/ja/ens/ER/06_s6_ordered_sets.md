---
book: ens
book_title: Theory of Sets
chapter: ER
chapter_title: SUMMARY OF RESULTS
section: 6
section_title: Ordered sets
lang: ja
source: ens-i-iv
source_edition: 2004, Springer
book_pages: 373-380
pdf_pages: 0378-0385
extraction: ocr
statements: 0
exercises: 0
content_sha256: 902f0250517ef7389cc3a8d0f54102659f1bbb8ca0478f5649be0348cc8d29df
translated_from: content/en/ens/ER/06_s6_ordered_sets.md
translation_method: google
source_content_sha256: 971a0a96b2a9c9ae41e13935799a40e904d52151f935272d34c3c4e23f4b84cc
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 74e861b6309cef067939d398c44764d6bfbfd2242913c257c7dbc340152bbeee
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 6. 順序集合

1. 集合 E の 2 つの一般的な元 x, y の間の関係 $\omega\{x,y\}$ は、次の 2 つの条件を満たす場合、E では順序関係であると言われます。
(a) 関係 「$\omega\{x,y\}$ と $\omega\{y,z\}$」は「$\omega\{x,z\}$」 (推移性) を意味します。
(b) 関係 「$\omega\{x,y\}$ と $\omega\{y,x\}$」は「$x=y$」に相当します。
条件 (b) は、$\omega$ が再帰的であることを意味します。

C を対 $(x,y)$ の性質として関係 $\omega\{x,y\}$ によって定義される $E\times E$ の部分集合とします。この場合、条件 (a) と (b) はそれぞれ次と等価です: (a') $C \circ C \subset C$; (b')$C \cap \overline{C}^{-1} = \Delta$。これらは $C \circ C = C$ を意味します。

集合 $E$ 上の特定の順序関係を考慮すると、$E$ はこの関係によって順序付けられ、関係定義する順序構造 (cf.) §8) (または注文) $E$。

$\omega\{x,y\}$ が $E$ に順序関係であれば、$\omega^{-1}\{x,y\}$ も同様です。これら 2 つの順序関係とその順序定義するは、互いに反対であると言われています。

$\omega\{x,y\}$ を $E$ の順序関係とし、$A$ を $E$ のいずれかの部分集合とします。 $A$ の 2 つの一般的な元 $x,y$ の間の関係 $\omega\{x,y\}$ は、$A$ では順序関係となり、$A$ での定義するの順序付けは、次で定義された順序付けによって引き起こされると言われます。 $E$の$\omega\{x,y\}$。 $E$ に与えられた順序は、$A$ に誘導された順序の拡大であると言われます。

$E$ の 2 つの汎用元 $x,y$ の間の再帰的かつ推移的な関係 $\overline{\omega}\{x,y\}$ は、$E$ の予約注文関係と呼ばれます。 関係「$\overline{\omega}\{x,y\}$と$\overline{\omega}\{y,x\}$」は$E$の同値関係$R$で、$\overline{\omega}\{x,y\}$はこの関係と互換性があります（$x$と$y$では）。 移行から商 ($x$ と $y$ に関して)、集合 $E/R$ 順序関係に$\overline{\omega}\{x,y\}$ 誘導するが関連付けられていると言われています。 $\overline{\omega}\{x,y\}$。予約注文関係が付与された集合は、予約注文集合と呼ばれます。

2. 包含関係 “$Y \subset X$” は、集合 $E$ の部分集合 $\mathfrak{P}(E)$ の集合に順序関係が含まれます。

$E$ と $F$ が 2 つの集合であり、区別できる場合とそうでない場合、 関係 「$g$ 拡大する $f$」は、すべての集合上の順序関係になります。 $E$の部分集合の写像が$F$に。

ナチュラル整数 [^1]の集合 $\mathbf{N}$は、関係「$x \leq y$」でオーダーされます。

3. この最後の例から類推すると、集合 $E$ が関係 $\omega\{x,y\}$ で順序付けされる場合、関係 $\omega\{x,y\}$ を $x \leq y$ または $y \geq x$ で表すと便利なことがよくあります。これらの関係は、「$x$ が $y$ より小さい」、または「$y$ が $x$ より大きい」[^2] と読み取られます。 関係「$x<y$」と「$y>x$」（「$x$は厳密に$y$より小さい」、または「$y$は厳密に$x$より大きい」と読みます）は、定義までは「$x\leq y$および$x\neq y$」と同等です。

関係 「$x\leq y$」は「$x<y$ または $x=y$」と同等です。 関係 「$x\leq y$ と $y<z$」は「$x<z$」を意味します。同様に、「$x<y$ と $y\leq z$」は「$x<z$」を意味します。

4. 関係「$\leq$」によって順序付けられた集合 E の部分集合 X は、すべての $x\in X$ とすべての $y\in X$ について、$x\leq y$ または $y\leq x$ (または同等に、$x<y$ または $x=y$ のいずれか) がある場合、この関係によって *完全に順序付け* されていると言われます。 $x>y$、これら 3 つの関係は相互に排他的です)。
順序付きセットの空のサブセットは常に完全に順序付けされています。 集合 $\mathbf{N}$ と関係 $x\leq y$ の場合のように、集合 E 全体が完全に順序付けされる場合があります。
完全に順序付けされた集合のすべての部分集合は、誘導順序付けによって完全に順序付けされます。
順序付き集合 E で、$a$ と $b$ が 2 つの元である場合、$a\leq b$、E の部分集合元 $x$ のからなるが$a\leq x\leq b$ を *closed 区間と呼びます。左側の端点 a と右側の端点 b* を持ち、$[a,b]$ で示されます。 $a\leq x<b$ (それぞれ $a<x\leq b$) のようなすべての $x\in E$ の集合は、端点 $a$ と $b$ を持つ *右側の半開* (それぞれ *左側*) の区間と呼ばれ、 $[a,b[$ (それぞれ $]a,b]$) で表されます。 $a<x<b$ のようなすべての $x\in E$ のセットは、端点 $a$ と $b$ を持つ *開区間* と呼ばれ、$]a,b[$ で表されます。
$x\leq a$ (それぞれ $x<a$) のようなすべての $x\in E$ の集合は *closed* (それぞれ *open*) *左側に境界がなく、右側の端点 a* の区間と呼ばれ、 $] \leftarrow,a]$ (それぞれ $]\leftarrow,a[$) で表されます。同様に、$x\geq a$ (それぞれ $x>a$) であるすべての $x\in E$ の集合は、左側の端点 a* を持つ、右側に境界のない *closed* (それぞれ *open*) *区間と呼ばれ、$[a,\rightarrow[$ (それぞれ $]a,\rightarrow[$) で表されます。 最後に、E 自体を *両方向に境界のない開いた区間* と見なし、それを $]\leftarrow,\rightarrow[$ で表します。

5. X が順序付けられた集合 E の部分集合である場合、すべての $x\in X$ に対して $a\leq x$ となるような X の元 $a$ は最大 1 つあります。この性質に元$a$が存在するとき、それをX*の*最小元と呼びます。 同様に、すべての $x\in X$ に対して $x\leq b$ となる元 $b$ は最大 1 つ存在します。 $b$ が存在する場合、それは X* の *最大の元と呼ばれます。
*完全に順序付けされた集合 E* では、空ではないすべての *有限* 部分集合には最大の元と最小の元があり、それぞれ部分集合の *最大値と最小値* 元と呼ばれます。
空ではないすべての部分集合に少なくとも元が含まれる、順序付けられた集合は、*適切に順序付けされている*と言われます。 自然な整数の集合 $\mathbf{N}$ は整然としています。 $\mathbf{N}$ の部分集合は、それが有限で空でない場合に限り、 最大の元を持ちます。 選択公理を使用すると、すべての集合に適切な順序付け (*ゼルメロの定理*) が存在することが示されます。
包含順に並べられた集合 E の部分集合の集合 $\mathfrak{P}(E)$ では、$\mathfrak{F}$ の集合の交差が $\mathfrak{F}$ に属し、この交差が最小要素となる場合に限り、$\mathfrak{P}(E)$ の部分集合 $\mathfrak{F}$ が最小要素を持ちます。 同様に、$\mathfrak{F}$ は $\mathfrak{F}$ 属するから $\mathfrak{F}$ の集合の和集合である場合に限り、最大の元となり、この和集合は最大の元になります。
順序付けられた集合 E の部分集合 X は、各 $y\in E$ に対して $y\leq x$ (それぞれ $y\geq x$) となる $x\in X$ が存在する場合、E の *cofinal* (それぞれ *coinitial*) であると言われます。 順序付けられた集合 $E$ に最大の (それぞれ最小) 元があるということは、単一の元の $E$ からなるの余終点 (それぞれ最小) 部分集合が存在することを意味します。

6. $X$ を、順序付けられた集合 $E$ の部分集合とします。 $z<x$ が $X$ の *最小元* と呼ばれる元 $z\in X$ が存在しないようなすべての $x\in X$ 。 $z>y$ が $X$ の *極大元* と呼ばれる元 $z\in X$ が存在しないようなすべての $y\in X$ 。 極大元の集合 (または最小限の元の集合) は空である可能性があります。それは無限である可能性もあります。 $X$ に最小の元 $a$ がある場合、$a$ は $X$ の*唯一* 最小の元です。同様に、$X$ に最大の元 $b$ がある場合、$b$ は $X$ の*のみ* 極大元です。

7. $X$ を、順序付けられた集合 $E$ の部分集合とします。 元 $x\in E$ がすべての $z\in X$ に対して $z\leq x$ となる場合、$x$ は $X$ の *上界* と呼ばれます。同様に、すべての $z\in X$ に対して $z\geq y$ となる元 $y\in E$ は、$X$ の *下界* と呼ばれます。

部分集合 $X$ の上界の集合 (または下界の集合) は空の場合があります。 部分集合 $X$ の上限 (または下限) の集合が空ではないことを、*上に境界がある* (または *下に境界がある*) と言います。上下両方に有界のある集合は、単に*有界*であると言われます。 $X$ の上界より大きいすべての元は、$X$ の上界になります。 $X$ の下界未満のすべての元は、$X$ の下界になります。

部分集合 $X$ の上界のうち集合に最小の元 $a$ がある場合、$a$ は $X$ の *最小上界* または *最高* と呼ばれます。 $X$ の下界の集合に最大の元 $b$ がある場合、$b$ は、$X$ の *最大の下界* または *infimum* と呼ばれます。これらの境界が存在する場合、それらは定義によって一意であり、それぞれ $\sup_E X$ (または $\sup X$)、 $\inf_E X$ (または $\inf X$) で示されます。 $X$ に最大の元がある場合、それは最小の上界です。 $X$ に少なくとも元がある場合、それはその最大の下界になります。逆に、$X$ の最小の上界 (それぞれ最大の下界) が存在し、$X$ に属するが存在する場合、それは $X$ の最大の (それぞれ最小) 元になります。

$f$ を集合 $A$ の写像を $E$ にします。 $f(A)$ が上に境界がある場合 (それぞれ、下に境界があり、境界がある)、$f$ は *上に境界がある* (それぞれ *下に境界があり、境界がある*) と言われます。 $f(A)$ が $E$ に最小上界 (それぞれ最大の下界) を持つ場合、この境界は $f$ の *最小上界* (それぞれ *最大の下界*) と呼ばれ、次のように表されます。 $\sup_{x\in A} f(x)$ (それぞれ $\inf_{x\in A} f(x)$)。

8. $E$ のすべての *有限の空ではない * 部分集合が *上に有界* (または *下に有*) である事前順序付けされた集合 $E$ は、*右向き* (または *有向*) (それぞれ *左有向*) と言われます。

$E$ のすべての *有限の空でない* 部分集合が少なくとも上界と最大の下界を持つ、順序付けられた集合 $E$ を *格子* と呼びます。

包含順に並べた、任意の集合の部分集合の集合は *格子* です。完全に順序付けられたすべての集合は格子です。

9. 順序付けられた集合 E は、次の条件を満たす場合、*帰納的*であると言われます: *E のすべての完全に順序付けられた部分集合には上界* があります。

集合 $\mathfrak{P}(E)$ は包含順に並べられており、帰納的です。 f と g の間の関係「g は f を拡張する」によって順序付けされた場合、集合 E の部分集合の集合 F へのマッピングの集合も同様です。

帰納的集合の任意の部分集合は一般に帰納的ではありません。しかし、a が帰納的集合 E のいずれかの元である場合、E の部分集合からなるはすべての元 $x \in E$ となり、$x \geq a$ は帰納的になります。

10. 次の命題は、選択の公理を利用して証明され、*Zorn の補題* として知られています。

*すべての帰納的順序集合には、少なくとも 1 つの極大元があります。*

11. 包含順に並べた、集合 E の部分集合 $\mathfrak{P}(E)$ の集合では、E の部分集合の集合 $\mathfrak{F}$ の最小上界は、$\mathfrak{F}$ の集合の *和集合* です。 Zorn の補題を適用すると、次の結果が得られます。

*$\mathfrak{F}$ が集合の部分集合の集合である場合、$\mathfrak{F}$ の各部分集合 $\mathfrak{G}$ について、包含の関係によって完全に順序付けされ、$\mathfrak{G}$ の集合の和集合属するから $\mathfrak{F}$ の場合、$\mathfrak{F}$ には少なくとも 1 つの極大元* があります (つまり、属するから $\mathfrak{F}$ までの E の部分集合ですが、E 所属から $\mathfrak{F}$ の他の部分集合には含まれていません)。

性質 “$X \in \mathfrak{F}$” が性質 “X のすべての *有限* 部分集合と * 等しい* 場合、集合の部分集合の集合 $\mathfrak{F}$ は *有限指標* であると言われます属するから$\mathfrak{F}$」。この定義により、次の定理が得られます。

*有限指標の E の部分集合のすべての集合には、少なくとも 1 つの極大元があります。*

12. A の一般的な元の間の関係 $x \leq y$ が $f(x) \leq f(y)$ を意味する場合、順序付き集合 E の部分集合 A の写像 f を順序付き集合に変換すると、F は *増加する* (それぞれ *減少する*) であると言われます。 (それぞれ $f(y) \leq f(x)$)。したがって、A 上のすべての定数写像は、増加すると減少するの両方であり、A が (右または左) 方向に向いている場合、逆は真になります。

関係 $x < y$ が $f(x) < f(y)$ (それぞれ $f(x) < f(y)$) を意味する場合、写像 f は *真に増加する* (それぞれ *真に減少する*) であると言われます。

E が *完全順序付け* の場合、E の部分集合 A のすべての *真に増加する* (または *真に減少する*) 写像が順序付けされた集合 F に入るのは *単射的* です。

I が添字の *順序付けられた* 集合である場合、集合 E の部分集合のファミリー $(X_i)_{i \in I}$ は、I の写像 $i \to X_i$ が *増加する* (それぞれ *減少する*) であると言われます。 $\mathfrak{P}(E)$ を包含順に並べると、増加する (それぞれ減少する) になります。

13. I を有向集合とし、$(E_\alpha)_{\alpha \in I}$ を I でインデックス付けされた集合のファミリーとします。 $\alpha \leq \beta$ のような I の添字の各対 $(\alpha, \beta)$ について、$f_{\beta \alpha}$ を写像 *of* $E_\alpha$ *into* $E_\beta$ とし、関係 $\alpha \leq \beta \leq \gamma$ が意味すると仮定します。 $f_{\gamma \alpha} = f_{\gamma \beta} \circ f_{\beta \alpha}$。

F を集合 $(E_\alpha)_{\alpha \in I}$ の家族の和とします。言葉の乱用により、F の対応する部分集合で $E_\alpha$ を同一視するとします。F に 2 つの元 x と y が与えられると、R $\{x, y\}$ を次の関係とします (ここで、$\alpha$ と $\beta$ は元を表します) $x\in E_\alpha$ と $y\in E_\beta$ のような $I$): 「$\gamma\geq\alpha$ と $\gamma\geq\beta$ と $f_{\gamma\alpha}(x)=f_{\gamma\beta}(y)$ のような $\gamma\in I$ が存在します。」すると、$R$は$F$の同値関係になります。 $E$ を商集合 $F/R$ とし、$f$ を標準写像 $F\to F/R$ とします。 集合 $E$ は、写像* $(f_{\beta\alpha})$ の家族に対して*直系の極限 $(E_\alpha)_{\alpha\in I}$ と呼ばれ、$f$ ～ $E_\alpha$ のうちの制限 $f_\alpha$ は、 *$E_\alpha$の標準写像を$E$に。 $\alpha\leq\beta$はいつでも$f_\beta\circ f_{\beta\alpha}=f_\alpha$になります。私たちは書きます

$$
E=\underset{\longrightarrow}{\lim}\,(E_\alpha,f_{\beta\alpha})
$$

または、混乱の危険がない場合は、単に $E=\underset{\longrightarrow}{\lim}\,E_\alpha$ と入力します。言葉の乱用により、対 $((E_\alpha),(f_{\beta\alpha}))$ は、* $I$ に対して集合の *直接系と呼ばれます。

$f_{\beta\alpha}$ が単射であれば、$f_\alpha$ も単​​射です。この場合、通常は同一視する $E_\alpha$ と $f_\alpha(E_\alpha)$ となるため、$E$ は $E_\alpha$ の *和集合* と見なされます。逆に、集合 $E'$ が部分集合の家族 $(E'_\alpha)_{\alpha\in I}$ の和集合である場合、関係 $\alpha\leq\beta$ は $E'_\alpha\subset E'_\beta$ を意味し、$j_{\beta\alpha}$ が ($\alpha\leq\beta$ の場合) 標準単射を示す場合、 $E'_\alpha$を$E'_\beta$にすると、$E'$で同一視する$\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$、$E'_\alpha$の標準写像を$\underset{\longrightarrow}{\lim}\,(E'_\alpha,j_{\beta\alpha})$に、$E'_\alpha$の標準単射を$E$にすることができます。

より一般的には、$(E_\alpha,f_{\beta\alpha})$ を $I$ に対する集合の直接系とし、各 $\alpha\in I$ について、$g_\alpha$ を $E_\alpha$ の写像から集合 $E'$ とし、関係 $\alpha\leq\beta$ とします。 $g_\beta\circ f_{\beta\alpha}=g_\alpha$ を意味します。 次に、すべての $\alpha\in I$ に対して $g_\alpha=g\circ f_\alpha$ となるように、$E=\underset{\longrightarrow}{\lim}\,E_\alpha$ から $E'$ への一意のマッピング $g$ が存在します。 写像 $g$ は、$E'$ が $g_\alpha(E_\alpha)$ の和集合である場合にのみ全射的です。 写像 $g$ は、各 $\alpha\in I$、関係 $x\in E_\alpha$、$y\in E_\alpha$、$g_\alpha(x)=g_\alpha(y)$ が $f_{\beta\alpha}(x)=f_{\beta\alpha}(y)$ となるような $\beta\geq\alpha$ が存在することを暗示している場合にのみ単射的です。 $g$ が全単射である場合、$E'$ は$E_\alpha$ の直接の極限と同一視されることがあります。

$(A_\alpha,\varphi_{\beta\alpha})$ と $(B_\alpha,\psi_{\beta\alpha})$ を、同じ添字集合 $I$ に対する集合の 2 つの直接系とします。 $A=\underset{\longrightarrow}{\lim}\,(A_\alpha,\varphi_{\beta\alpha})$、$B=\underset{\longrightarrow}{\lim}\,(B_\alpha,\psi_{\beta\alpha})$、そしてそれぞれの $\alpha\in I$ について、$\varphi_\alpha$ (それぞれ $\psi_\alpha$) は、$A_\alpha$ から $A$ への標準写像 (それぞれ $B_\alpha$ から $B$) を表します。それぞれの $\alpha\in I$ について、$u_\alpha$ を $A_\alpha$ の写像を $B_\alpha$ にすると、$\alpha\leq\beta$ のときは常に $u_\beta\circ\varphi_{\beta\alpha}=\psi_{\beta\alpha}\circ u_\alpha$ になります。家族 $(u_\alpha)$ は、* $(A_\alpha,\varphi_{\beta\alpha})$ の写像の * $(B_\alpha,\psi_{\beta\alpha})$ への * 直接系と呼ばれます。これらの条件の下には、すべての $\alpha\in I$ に対して $u\circ\varphi_\alpha=\psi_\alpha\circ u_\alpha$ となるように一意な写像 $u:A\to B$ が存在します。 写像 $u$ は、* $u_\alpha$ の * 直接極限と呼ばれ、混同の危険がない限り、$u=\underset{\longrightarrow}{\lim}\,u_\alpha$ と書かれます。 $(C_\alpha,\theta_{\beta\alpha})$ を $I$ に対する集合の他の直接系とし、$(v_\alpha)$ を $(B_\alpha,\psi_{\beta\alpha})$ の写像の $(C_\alpha,\theta_{\beta\alpha})$ に対する直接系とし、$v=\underset{\longrightarrow}{\lim}\,v_\alpha$ とします。それから

$$
\underset{\longrightarrow}{\lim}\,(v_\alpha\circ u_\alpha)=v\circ u.
$$

上記の記法をそのままにして、$D_\alpha=A_\alpha\times B_\alpha$と$\omega_{\beta\alpha}=\varphi_{\beta\alpha}\times\psi_{\beta\alpha}$とします。すると、家族$(D_\alpha,\omega_{\beta\alpha})$は集合の直接系になります。 $D=\underset{\longrightarrow}{\lim}\,(D_\alpha,\omega_{\beta\alpha})$、$\omega_\alpha$を$D_\alpha$の標準写像を$D$、$D'=A\times B$、$\omega'_\alpha=\varphi_\alpha\times\psi_\alpha$とします。次に、すべての $\alpha\in I$ に対して $f\circ\omega_\alpha=\omega'_\alpha$ となるような、一意の全単射 (正規と呼ばれる) $f:D\to D'$ が存在します。通常、直接極限の同一視する積 $D'$ と、積 $D_\alpha$ の直接極限 $D$ とします。

$J$ を $I$ の最終値部分集合とします。その後、$J$も指示されます。 $( (E_\alpha)_{\alpha\in I},(f_{\beta\alpha})_{\alpha,\beta\in I})$ が $I$ に対して集合の直接系である場合、$( (E_\alpha)_{\alpha\in J},(f_{\beta\alpha})_{\alpha,\beta\in J})$ は $J$ に対して集合の直接系です。 $E'$ を直接の極限とし、$f'_\alpha$ を $E_\alpha$ の標準写像をすべての $\alpha\in J$ の $E'$ にします。次に、すべての $\alpha\in J$ とすべての $x\in E_\alpha$ に対して $g(f'_\alpha(x))=f_\alpha(x)$ となるような一意な写像 $g:E'\to E$ が存在します (ここで、$f_\alpha$ は $E_\alpha$ の標準写像を $E$ に表します)。この写像は全単射であり、これにより通常 $E'$ は $E$ と識別されます。

14. $I$ を事前注文された集合とし、$(E_\alpha)_{\alpha\in I}$ を $I$ によってインデックス付けされた集合のファミリーとします。 $\alpha\leq\beta$ のような $I$ のインデックスの各ペア $(\alpha,\beta)$ について、$f_{\alpha\beta}$ を $E_\beta$ から $E_\alpha$ へのマッピングとし、関係 $\alpha\leq\beta\leq\gamma$ が $f_{\alpha\gamma}=f_{\alpha\beta}\circ f_{\beta\gamma}$ を意味すると仮定します。

$G$ を集合 $(E_\alpha)_{\alpha\in I}$ の家族の積とします。 $E$ を、$\alpha\leq\beta$ となるインデックス$\alpha,\beta$ のすべてのペアについて、すべての関係 $pr_\alpha x=f_{\alpha\beta}(pr_\beta x)$ を満たすすべての要素 $x$ で構成される $G$ のサブセットとします。 集合 $E$ は、写像 $(f_{\alpha\beta})$ の族に対する $(E_\alpha)_{\alpha\in I}$ 族の逆元極限と呼ばれ、$pr_\alpha$ から $E$ の制限 $f_\alpha$ は、標準写像と呼ばれます$E$ から $E_\alpha$ に。 $\alpha\leq\beta$ のときはいつでも $f_\alpha=f_{\alpha\beta}\circ f_\beta$ があります。 私たちは書きます

$$
E=\lim (E_\alpha,f_{\alpha\beta}),
$$

または単に

$$
E=\lim E_\alpha
$$

混乱を招く恐れがない場合。

言葉の乱用により、対 $((E_\alpha),(f_{\alpha\beta}))$ は、$I$ に対する集合の逆数系と呼ばれます。

すべての $E_\alpha$ が空でなく、すべての写像 $f_{\alpha\beta}$ が全射である場合でも、$E$ は空になる可能性があることに注意してください。

それぞれの $\alpha\in I$ について、$g_\alpha$ を集合 $E'$ の写像を $E_\alpha$ にすると、関係 $\alpha\leq\beta$ は $f_{\alpha\beta}\circ g_\beta=g_\alpha$ を意味します。 次に、すべての $\alpha\in I$ に対して $g_\alpha=f_\alpha\circ g$ となるように、$E'$ から $E$ への一意のマッピング $g$ が存在します。 $g$ が単射であるためには、$E'$ の個別の元 $x',y'$ のそれぞれの対に対して、$g_\alpha(x')\neq g_\alpha(y')$ となるような $\alpha\in I$ が存在する必要があって十分です。

$(A_\alpha,\varphi_{\alpha\beta})$ と $(B_\alpha,\psi_{\alpha\beta})$ を、同じ添字集合 $I$ に対する集合の 2 つの逆数系とします。 $A=\lim(A_\alpha,\varphi_{\alpha\beta})$、$B=\lim(B_\alpha,\psi_{\alpha\beta})$ とし、それぞれの $\alpha\in I$ について、$\varphi_\alpha$ (それぞれ $\psi_\alpha$) を $A$ の $A_\alpha$ の標準写像 (それぞれ $B$ を $B_\alpha$ に) とします。 それぞれの $\alpha\in I$ について、$u_\alpha$ を $A_\alpha$ の写像を $B_\alpha$ にすると、$\alpha\leq\beta$ のときは常に $\psi_{\alpha\beta}\circ u_\beta=u_\alpha\circ\varphi_{\alpha\beta}$ になります。 ファミリ $(u_\alpha)$ は、$(A_\alpha,\varphi_{\alpha\beta})$ の写像を $(B_\alpha,\psi_{\alpha\beta})$ に反転したもの系と呼ばれます。 これらの条件の下には、すべての $\alpha\in I$ に対して $\psi_\alpha\circ u=u_\alpha\circ\varphi_\alpha$ となるように一意な写像 $u:A\to B$ が存在します。 写像 $u$ は、$u_\alpha$ の逆数極限と呼ばれ、混乱の危険がない場合は $u=\underset{\longleftarrow}{\lim}\,u_\alpha$ と書かれます。 $(C_\alpha,\theta_{\alpha\beta})$ を $I$ に対する別の集合の逆系とし、$v_\alpha$ を $(B_\alpha,\psi_{\alpha\beta})$ から $(C_\alpha,\theta_{\alpha\beta})$ への写像の逆系とし、$v=\underset{\longleftarrow}{\lim}\,v_\alpha$ とします。 次に、$\underset{\longleftarrow}{\lim}\,(v_\alpha\mathbin{\circ}u_\alpha)=v\mathbin{\circ}u$です。
$J$ を $I$ の余終点部分集合とし、$J$ が ($I$ から誘導される順序付けに関して) *指示* されていると仮定します。 $((E_\alpha)_{\alpha\in I},(f_{\alpha\beta})_{\alpha,\beta\in I})$ が $I$ に対する集合の逆数系で、極限 $E$ の逆数である場合、$((E_\alpha)_{\alpha\in J},(f_{\alpha\beta})_{\alpha,\beta\in J})$ は $J$ に対する集合の逆数系でもあります。 $E'$ をその逆数極限とし、$f'_\alpha$ を $E'$ の標準写像を $E_\alpha$ に変換します。ここで、$\alpha\in J$ です。 それぞれの $x\in E$ を $g(x)=(f_\alpha(x))_{\alpha\in J}\in E'$ とします (ここで、$f_\alpha$ は $E$ の標準写像を $E_\alpha$ に変換することを示します)。 この場合、$g$ は $E$ の $E'$ への *全単射* であり、これにより、$E'$ は通常 $E$ と識別されます。

[^1]: この結果概要の点の見解に従って、既知のとおり理論または整数を想定します。 しかし、この理論が集合の理論を構築するために必要であると考えるべきではありません。読者は、章 III を参照すると、逆に、集合の理論の結果から、整数が定義でき、その既知の特性がすべて証明できることがわかります。 In our terminology, $0$ belongs to $\mathbf{N}$.
[^2]: Thus, in our terminology, “less than” and “greater than” do not exclude “equal to”.
