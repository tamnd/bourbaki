---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 16
section_title: Other Descriptions of the Brauer Group
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.285-A VIII.333
pdf_pages: 0302-0350
extraction: native+ocr
subsections:
    - "no": 1
      title: $\tau$-Extensions of Groups
      page: 285
      pdf_page: 302
    - "no": 2
      title: Inverse Image of a $\tau$-Extension
      page: 287
      pdf_page: 304
    - "no": 3
      title: Direct Image of a $\tau$-Extension
      page: 289
      pdf_page: 306
    - "no": 4
      title: Group Law on the Classes of $\tau$-Extensions
      page: 293
      pdf_page: 310
    - "no": 5
      title: Cohomological Description
      page: 295
      pdf_page: 312
    - "no": 6
      title: Restriction and Corestriction
      page: 299
      pdf_page: 316
    - "no": 7
      title: Galois Algebras
      page: 304
      pdf_page: 321
    - "no": 8
      title: Actions on Galois Algebras
      page: 312
      pdf_page: 329
    - "no": 9
      title: Cross Products
      page: 314
      pdf_page: 331
    - "no": 10
      title: Application to the Brauer Group
      page: 317
      pdf_page: 334
    - "no": 11
      title: Index and Exponent
      page: 322
      pdf_page: 339
statements: 63
exercises: 17
content_sha256: 8a7d8d64d56cfbd43ef248595f01c0ddabad16ac9cab1e64c80eb819b9208886
translated_from: content/en/alg/VIII/16_s16_other_descriptions_of_the_brauer_group.md
translation_method: google
source_content_sha256: 67633b439572bf5a4dcc4c35edb70b8c99883cdac1bfa5ce829e7e8f5be14d83
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: f6f36fa657cd61a8594e542035304bf508eb94af4cad335a1bc1599d1eee6c85
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 16。その他記述/ブラウアー群

この切断で、Fがアーベル群とFの$g$自己同型であれば、$g(f)$に$g\cdot f$と書きます。

### 1. $\tau$-群の拡張機能

この小節では、乗算的に書かれた群 G、アーベル群 F、および G からの群準同型 $\tau$ を F の自己同型群 Aut(F) に固定します。G の単位元を $e$ で、F の単位元をそれぞれ表します。 1.

(I, §6, No. 1, p. 65) を思い出してください。F による G の拡大 $\mathscr{E}$ はトリプル $(\Gamma , \iota , \pi )$ で、Γ は群、$\pi : \Gamma \rightarrow G$ は全射準同型、$\iota$ は F から Γ までの単射準同型です。イム($\iota$ ) $=$ カー($\pi$ )。 $\mathscr{E}= (\Gamma , \iota , \pi )$ をそのような拡大とします。 $\gamma \in \Gamma$、写像 $\varphi_{\gamma}: F\rightarrow F$ ごとに、次のように定義されます。

$$
\iota (\varphi_{\gamma}(f)) =\gamma \iota (f)\gamma^{-1}
$$

$f\in F$ は F の自己同型です。F は可換なので、すべての $f\in F$ に対して、$\iota (f)$ によって定義される自己同型は F 上で恒等写像になります。 移行から商までにより、G から Aut(F) まで特徴付けられた準同型 Int$_{\mathscr{E}}$ が得られます。によって

$\gamma \iota (f)\gamma^{-1}=\iota$(整数$_{\mathscr{E}}(\pi (\gamma ))\cdot f$)

$\gamma \in \Gamma$ と $f\in F$ の場合。

F による G の $A\tau$ 拡張は、Int$_{\mathscr{E}}$ が $\tau$ に等しくなるように拡大 $\mathscr{E}= (\Gamma , \iota , \pi )$ であり、他の語では、関係を満たす

$$
\gamma \iota (f)\gamma^{-1}=\iota (\tau (\pi (\gamma ))\cdot f) \tag{1}
$$

$\gamma \in \Gamma$ と $f\in F$ の場合。 $\mathscr{E}= (\Gamma , \iota , \pi )$ と $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ が $\tau$ 拡張である場合、$\mathscr{E}$ から $\mathscr{E}'$ までの $\tau$ 拡張の射は、$\mathscr{E}$ から $\mathscr{E}'$ までの拡大の射です。 (I, §6, No. 1、p. 65)、つまり、群準同型 $u: \Gamma \rightarrow \Gamma '$ は、$\pi '\circ u=\pi$ と $\iota '=u\circ \iota$ になります。 $\tau$ 拡張子形は、すべての射が同型 (集合理論、IV, §1, No. 5、p. 264、I, §6, No. 1) である構造の種であることに注意してください。 p. 66、命題 1)。 Iso で示す$_{\tau}(\mathscr{E},\mathscr{F})$ 関係

「$\mathscr{E}$ と $\mathscr{F}$ は同型の $\tau$ 拡張子です。」

これは同値関係です。 拡大 $\mathscr{E}$ の類は、Iso$_{\tau}($集合理論、II, §6, No. 6、p. 122 の $\mathscr{E}$ に相当するオブジェクトの類です。

#### 補題 1 {#alg-viii-s16-lem-1 .statement tag=00I9}

関係

「$\alpha$ は、Iso$_{\tau}$ の $\tau$ 拡張機能の類です」

$\alpha$で集団化しています。

集合 $E_0= F\times G$、そして $f\in F$ の場合は $\iota_0(f) = (f, e)$ 、$(f, g)\in F\times G$ の場合は $\pi_0(f, g) =g$ によって定義される写像 $\iota_0: F\rightarrow E_0$ と $\pi_0: E_0\rightarrow G$ を考えてみましょう。 $\mathscr{E}= (\Gamma , \iota , \pi )$ を F による G の $\tau$ 拡張とします。 写像 $\pi$ は全射なので、 切断 $\sigma : G\rightarrow \Gamma$ は $\sigma (e) =e$ になります。 写像 $u: (f, g)\mapsto \iota (f)\sigma (g)$ $F\times G$ から Γ までは全単射です。 構造の譲渡で得た群法則を$F\times G$に贈呈させていただきます。トリプル $(E_0, \iota_0, \pi_0)$ は、$\mathscr{E}$ と同型の $\tau$ 拡張です。 補題 1 は、集合理論、II, §6, No. 6、p. 122 の後に続きます。

関係 Iso$_{\tau}$ の Ex$_{\tau}(G,F)$ 集合の類の $\tau$ の拡張子で表します。

#### 例 1 {#alg-viii-s16-n1-exa-1 .statement tag=00IA}

外部半直積 $(F\times_{\tau}G, i, p)$ (I, §6, No. 1、p. 66、命題 3) は $\tau$ 拡張です。それを$\mathscr{I}_{\tau}$で表します。 $\tau$-拡張が $\tau$-拡張 $\mathscr{I}_{\tau}$ と同型である場合、それは半自明であると言います。

#### 例 2 {#alg-viii-s16-n1-exa-2 .statement tag=00IB}

$i\in  \{1,2\}$の場合は、$F_i$の$G_i$から自己同型群までの群$G_i$、アーベル群$F_i$、群準同型$\tau_i$をとります。によって定義される $\tau_1\times \tau_2: G_1\times G_2\rightarrow$ Aut(F$_1\times F_2$) 準同型で表します

$$
(\tau_1\times \tau_2)(g_1, g_2)\cdot (f_1, f_2) = (\tau_1(g_1)\cdot f_1, \tau_2(g_2)\cdot f_2)
$$

$g_1\in G_1,g_2\in G_2,f_1\in F_1$ と $f_2\in F_2$ の場合。 $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ を $G_1$ の $F_1$ による $\tau_1$ 拡張とし、$\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ を $G_2$ の $F_2$ による $\tau_2$ 拡張とします。 この場合、トリプル $(\Gamma_1\times \Gamma_2, \iota_1\times \iota_2, \pi_1\times \pi_2)$ は $G_1\times G_2$ の $F_1\times F_2$ による $\tau_1\times \tau_2$ 拡張です。それは、拡大 $\mathscr{E}_1$ および $\mathscr{E}_2$ の外部積と呼ばれ、$\mathscr{E}_1\times \mathscr{E}_2$ で示されます。

### 2. $\tau$ 拡張機能の逆像

G と $G'$ を群とします。 F をアーベル群とし、$\tau : G\rightarrow$ Aut(F) と $u: G'\rightarrow G$ を群準同型とします。 群準同型 $\tau '=\tau \circ u: G'\rightarrow$ Aut(F) を考え、$\pi$ と $u$ (I, §4, No. 8, p. 46) に対するファイバー 積 $\Gamma \times_GG'$ を $\Gamma '$ で表します。 It is the subgroup of $\Gamma \times G'$ consisting of the pairs $(\gamma , g')$ such that $\pi (\gamma ) =u(g')$. $\iota ': F\rightarrow \Gamma '$ を $\alpha \in F$ に対して $\iota '(\alpha ) = (\iota (\alpha ), e)$ によって与えられる群準同型とし、2 番目の射影を $\pi ': \Gamma '\rightarrow G'$ で表すとします。 この場合、射 $\iota '$ は単射的であり、$\pi$ はであるため、射 $\pi '$ は全射的であり、$\iota '$ 一致するの像は $\pi '$ の核となります。 さらに、$\alpha \in F$ と $\gamma '= (\gamma , g)\in \Gamma '$ ごとに、関係が得られます。

$$
\gamma '\iota '(\alpha )\gamma^{'-1}= (\gamma , g)(\iota (\alpha ), e)(\gamma , g)^{-1}= (\iota (\tau (\pi (\gamma )).\alpha ), e) =\iota '(\tau '(\pi '(\gamma ')).\alpha )
$$

従って、$(\Gamma ', \iota ', \pi ')$ は F による $G'$ の $\tau '$ 拡張です。 $\mathscr{E}$の逆像を$u$と呼び、$u^*(\mathscr{E})$で表します。最初の射影は群準同型 $\varphi : \Gamma '\rightarrow \Gamma$ であり、これを正規と呼びます。

#### 命題 1 {#alg-viii-s16-prop-1 .statement tag=00IC}

次の図式が通勤しています:

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

(2)

$\varphi u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

Moreover, if $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ is a $\tau '$-extension and $\varphi_1: \Gamma '_1\rightarrow \Gamma$ is a group homomorphism such that the diagram

F $^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

通勤する場合、$\mathscr{E}_1'$ から $u^*(\mathscr{E})$ までの $\tau '$ の内線番号一意な準同型 $\psi$ が存在し、$\varphi_1=\varphi \circ \psi$ になります。

最初の図式の可換性は、$\varphi$の定義から続きます。 $\psi$の存在と一意性は、以下の補題2から続きます。

#### 補題 2 {#alg-viii-s16-lem-2 .statement tag=00ID}

$F'_1$ をアーベル群とし、$w: F'_1\rightarrow$ F と $\tau_1: G'\rightarrow$ Aut(F$'_1$) を群準同型とします。

$$
w(\tau_1(g)(f)) =\tau (u(g))(w(f))
$$

$f\in F'_1$ と $g\in G'$ ごとに。 $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ を、$F'_1$ と $\varphi_1: \Gamma '_1\rightarrow \Gamma$ 群準同型による $G'$ の $\tau_1$ 拡張とし、次の図式が交換するようにします。

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$w\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

すると、図式のような一意な群準同型 $\psi : \Gamma '_1\rightarrow \Gamma '$ が存在します。

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi_1'}$ // $G'$

$w\psi$

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

通勤と$\varphi_1=\varphi \circ \psi$。

群準同型 $\psi : \Gamma '_1\rightarrow \Gamma '$ が望ましい特性を持っている場合、関係を満たします。

$$
\psi (\gamma ) = (\varphi \circ \psi (\gamma ), \pi '\circ \psi (\gamma )) = (\varphi_1(\gamma ), \pi '_1(\gamma ))
$$

$\gamma \in \Gamma '_1$ごとに。逆に、$\gamma \mapsto (\varphi_1(\gamma ), \pi_1'(\gamma ))$ によって定義される $\Gamma '_1$ から $\Gamma \times G'$ までの群準同型は、$\gamma \in \Gamma '_1$ ごとに $\pi \circ \varphi_1(\gamma ) =u\circ \pi_1'(\gamma )$ となるため、ファイバー 積 $\Gamma \times_GG'$ に値が含まれます。

#### 系 1 {#alg-viii-s16-lem-2-cor-1 .statement tag=00IE}

$\mathscr{E}_1$ と $\mathscr{E}_2$ を G による F の $\tau$ 拡張とし、$\psi$ を $\mathscr{E}_1$ から $\mathscr{E}_2$ までの $\tau$ の拡張の射とします。それぞれ$\varphi_1($で表します。 $u^*(\mathscr{E}_1) ($の場合は$\varphi_2)$ 標準準同型 $u^*(\mathscr{E}_2))$。次に、$\varphi_2\circ u^*(\psi ) =\psi \circ \varphi_1$ のように、$u^*(\psi )$ で示される、$u^*(\mathscr{E}_1)$ から $u^*(\mathscr{E}_2)$ までの $\tau '$ 拡張の一意な準同型が存在します。

命題を適用する 1 ～ $\psi \circ \varphi_1$ で十分です。

したがって、$\tau '$ 拡張子 $u^*(\mathscr{E})$ の類は、$\mathscr{E}$ の類にのみ依存します。また、$\tau$ 内線 $\mathscr{E}$ の類を $\tau '$ 内線 $u^*(\mathscr{E})$ の類に送信する $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G',F)$ 写像とも表します。

#### 系 2 {#alg-viii-s16-lem-2-cor-2 .statement tag=00IF}

$u': G''\rightarrow G'$ を群準同型とし、$\mathscr{E}$ を F による G の $\tau$ 拡張とし、集合 $\tau ''=\tau '\circ u'$ とし、それぞれ $\varphi ($ で表します。 $\varphi ',\varphi '')$ 標準準同型は、$\tau '$ 拡張子 $u^*(\mathscr{E}) ($ に関連付けられています。 $\tau ''$-内線 $u^{'*}(u^*(\mathscr{E}))$、$\tau ''$-内線 $(u\circ u')^*(\mathscr{E}))$。そして、$\tau ''$-延長$u^{'*}(u^*(\mathscr{E}))$から$\tau ''$-延長$(u\circ u')^*(\mathscr{E})$まで$\varphi ''\circ \psi =\varphi \circ \varphi '$となる一意な準同型$\psi$が存在します。

#### 例 {#alg-viii-s16-n2-exa-1 .statement tag=00RI}

H を G の部分群と $j: H\rightarrow G$ 標準単射とします。次に、すべての $\tau$ 拡張 $\mathscr{E}= (\Gamma , \iota , \pi )$ について、 $\tau \circ j$ 拡張 $j^*(\mathscr{E})$ は $(\overset{-1}{\pi}(H), \iota ', \pi ')$ と同型であり、ここで $\iota ': F\rightarrow \overset{-1}{\pi}(H)$ (それぞれ $\pi ':\overset{-1}{\pi}(H)\rightarrow H$) は群準同型 $f\mapsto \iota (f)$ (それぞれ $\gamma \mapsto \pi (\gamma )$) です。より一般的には、群準同型 $u: G'\rightarrow G$ が単射である場合、標準準同型 $\varphi$ は像 $\overset{-1}{\pi}(u(G'))$ と単射です。

### 3. $\tau$ 拡張機能の直像

Gを群、Fと$F'$をアーベル群、$\tau$（それぞれ$\tau '$）をGからFの自己同型群（それぞれ$F'$）までの群準同型、$v: F\rightarrow F'$を群準同型そのような

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{3}
$$

$g\in G$ と $f\in F$ ごとに。 $\mathscr{E}= (\Gamma , \iota , \pi )$ を F による G の $\tau$ 拡張とする。$\widetilde{\Gamma}$ を外部半直積 $F'\times_{\tau'\circ\pi}\Gamma$ とする。 $\widetilde{\imath}: F'\rightarrow \widetilde{\Gamma}$ 準同型 $f\mapsto (f, e)$ と最初の射影を $\widetilde{p}:\widetilde{\Gamma}\rightarrow \Gamma$ で表します。 $j: F\rightarrow \widetilde{\Gamma}$ を $f\mapsto (v(f), \iota (f)^{-1})$ によって定義される写像とします。 $\iota$の像は$\tau '\circ \pi$の核に含まれるので、写像$j$は群準同型です。 $\iota$ は単射なので単射です。 関係があります

$$
(f', \gamma )j(f)(f', \gamma )^{-1}= (f', \gamma )(v(f), \iota (f)^{-1})(f', \gamma )^{-1}
$$

$$
= (\tau '(\pi (\gamma ))\cdot v(f), \iota (\tau (\pi (\gamma ))\cdot f)^{-1}) \tag{4}
$$

$$
=j(\tau (\pi (\gamma ))\cdot f)
$$

$f\in F,\gamma \in \Gamma$ と $f'\in F'$ の場合。従って、$j$の像は、$\widetilde{\Gamma}$の通常の部分群になります。 $\widetilde{\Gamma}$の$\Gamma '$商、$j$の像で表します。 $\widetilde{\Gamma}$ から $\Gamma '$ および $\widetilde{\imath}$ までの標準全射の $\iota '$ 合成で表します。 準同型 $\pi \circ \widetilde{p}$ の核は、$j$ の含む像である積 $F'\times \iota$(F) です。 $\pi \circ \widetilde{p}$ から移行によって商から定義する $\pi ': \Gamma '\rightarrow G$ が群準同型として導き出されます。 $\iota$は単射なので、$j(F)$と$\widetilde{\imath}(F')$の共通部分は$\widetilde{\Gamma}$の単位元に還元されます。従って、$\iota '$ は単射法であることがわかります。 写像 $F'\times F$ から $F'\times \iota (F) =$ カー($\pi \circ \widetilde{p}$) によって与えられました

$$
(f', f)\longmapsto (f'v(f), \iota (f)^{-1})
$$

群同型です。 $\iota '$の像したがって、$\pi '$の核と一致する。 $\pi$ と $\widetilde{p}$ は全射なので、 $\pi '$ も全射です。これは、$\mathscr{E}'= (\Gamma ', \iota , \pi ')$ が G の $F'$ による $\tau '$ 拡張であることを証明します。 $\mathscr{E}$の直像を$v$と呼び、$v_*(\mathscr{E})$で表します。 $\gamma \mapsto (1, \gamma )$ によって与えられる $\widetilde{\Gamma}$ から $\Gamma '$ までの標準全射と Γ から $\widetilde{\Gamma}$ までの群準同型のうちの合成は、群準同型 $\varphi : \Gamma \rightarrow \Gamma '$ であり、これを正規と呼びます。

#### 命題 2 {#alg-viii-s16-prop-2 .statement tag=00IG}

上記の記法では、次の図式が通勤します。

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{5}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

$\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi_1')$ を $F'$ による G の $\tau '$ 拡張とし、次の図式が可換となるように $\varphi_1: \Gamma \rightarrow \Gamma '_1$ を群準同型とします。

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // G.

次に、$v_*(\mathscr{E})$ から $\mathscr{E}_1'$ までの $\tau '$ 拡張の一意な準同型 $\psi$ が存在し、$\varphi_1=\psi \circ \varphi$ になります。

最初の図式の可換性に構成が続きます。 $\psi$の存在と一意性は、以下の補題3から続きます。

#### 補題 3 {#alg-viii-s16-lem-3 .statement tag=00IH}

$G'_1$ を群とし、$w: G\rightarrow G'_1$ と $\tau_1: G'_1\rightarrow$ Aut(F$'$) を $\tau '=\tau_1\circ w$ となるように群準同型とします。 Let $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$ be a $\tau_1$-extension of $G'_1$ by $F'$, and let $\varphi_1: \Gamma \rightarrow \Gamma '_1$ be a group homomorphism such that the following diagram commutes:

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1w$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$。

すると、図式のような一意な群準同型 $\psi : \Gamma '\rightarrow \Gamma '_1$ が存在します。

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G

$\psi w$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$ 通勤と $\varphi_1=\psi \circ \varphi$。

任意の $(f, \gamma )\in F'\times \Gamma$ について、$\Gamma '$ の $(f, \gamma )$ の類を $(f, \gamma )$ で表します。 群準同型 $\psi : \Gamma '\rightarrow \Gamma '_1$ が望ましい特性を持っている場合、関係を満たします。

$$
\psi (f', \gamma )=\psi (\iota '(f')\varphi (\gamma )) =\iota '_1(f')\varphi_1(\gamma )
$$

$f'\in F'$ と $\gamma \in \Gamma$ ごとに。逆に、$(f, \gamma )\mapsto \iota '_1(f)\varphi_1(\gamma )$によって与えられる$F'\times_{\tau'\circ\pi}\Gamma$から$\Gamma '_1$までの写像$\widetilde{\psi}$は群準同型です。確かに、私たちは関係を持っています

$$
\iota '_1(f)\varphi_1(\gamma )\iota '_1(f')\varphi_1(\gamma ') =\iota '_1(f \tau_1(\pi '_1(\varphi_1(\gamma )))\cdot f')\varphi_1(\gamma \gamma ')
$$

$$
=\iota '_1(f \tau '(\pi (\gamma ))\cdot f')\varphi_1(\gamma \gamma ')
$$

$f, f'\in F'$ と $\gamma , \gamma '\in \Gamma$ の場合。 $\widetilde{\psi}$ の核含む $j$ の像は、$f\in F$ の $\iota '_1(v(f)) =\varphi_1(\iota (f))$ と、$\widetilde{\psi}$ から移行から商によって推定される射 $\psi$ が望ましい特性を持っているためです。

#### 注意 {#alg-viii-s16-n3-rem-1 .statement tag=00II}

群準同型である $\tau '$ 拡張の基礎となる $\tau '$ 拡張の構造と、Γ から群 $\Gamma '$ までの写像である定義する $\alpha$ マッピングの種を Σ で示します。 図式通勤:

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{6}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

命題 2 は、$v_*(\mathscr{E})$ が普遍的な対応する写像問題 (集合理論, IV, §3, No. 1, p. 284) の解であることを表します。

#### 系 1 {#alg-viii-s16-lem-3-cor-1 .statement tag=00IJ}

$\mathscr{E}_1$ と $\mathscr{E}_2$ を G の F による拡張 $\tau$ とし、$\psi$ を $\mathscr{E}_1$ から $\mathscr{E}_2$ までの $\tau$ 拡張の射とします。それぞれ$\varphi_1($で表します。 $v_*(\mathscr{E}_1) ($の場合は$\varphi_2)$ 標準準同型 $v_*(\mathscr{E}_2))$。次に、$v_*(\mathscr{E}_1)$ から $v_*(\mathscr{E}_2)$ までの $\tau '$ 拡張の一意な準同型が存在し、$v_*(\psi )$ で示され、$\varphi_2\circ \psi =v_*(\psi )\circ \varphi_1$ になります。

命題を適用する 2 ～ $\varphi_2\circ \psi$ までで十分です。

したがって、$\tau '$ 拡張子 $v_*(\mathscr{E})$ の類は、$\mathscr{E}$ の類にのみ依存します。また、$\tau$ 内線 $\mathscr{E}$ の類を $\tau '$ 内線 $v_*(\mathscr{E})$ の類に送信する $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ 写像とも表します。

#### 系 2 {#alg-viii-s16-lem-3-cor-2 .statement tag=00RJ}

命題の記法を保持します。 $F''$ をアーベル群とし、$\tau '': G\rightarrow$ Aut(F$''$) と $v': F'\rightarrow F''$ を群準同型とします。

$$
\tau ''(g)\cdot v'(f) =v'(\tau '(g)\cdot f)
$$

$g\in G$と$f\in F'$の場合。 $\mathscr{E}$ を F による G の $\tau$ 拡張とし、それぞれ $\varphi ($ で表します。 $\varphi ',\varphi '')$ 標準準同型は $v_*(\mathscr{E}) ($ に関連付けられています。 $v'_*(v_*(\mathscr{E}))$、$(v'\circ v)_*(\mathscr{E}))$。すると、G の $\tau ''$-延長 $v'_*(v_*(\mathscr{E}))$ から $F''$ で $\tau ''$-延長 $(v'\circ v)_*(\mathscr{E})$ までの一意な準同型 $\psi$ が存在し、$\varphi ''=\psi \circ \varphi '\circ \varphi$ になります。

#### 例 1 {#alg-viii-s16-n3-exa-1 .statement tag=00IK}

$j:\{1\} \rightarrow F$を標準単射とします。半自明な拡大 $\mathscr{I}_{\tau}$ は $j_*((G, i$、Id$_G))$ と同型であり、$i:\{e\} \rightarrow G$ は標準単射です。 $c: F\rightarrow F$ を定数準同型 $f\mapsto 1$ とし、$\mathscr{E}$ を $\tau$ 拡張とします。 $\tau$ 拡張子 $c_*(\mathscr{E})$ も $\mathscr{I}_{\tau}$ と同型です。

#### 例 2 {#alg-viii-s16-n3-exa-2 .statement tag=00IL}

E を G の作用の下で安定した F の部分群とします。F の $F'$ 商を E、$v: F\rightarrow F'$ 標準準同型、および $F'$ 上の G の $\tau ': G\rightarrow$ Aut(F$'$) 作用で表します。

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

$g\in G$ と $f\in F$ 用。 $\mathscr{E}= (\Gamma , \iota , \pi )$ を F による G の $\tau$ 拡張であるとします。そのとき、$\iota (E)$ は Γ の正規部分群であり、G の $F'$ による G の $\tau '$ 拡張 $v_*(\mathscr{E})$ は拡大 $(\Gamma /\iota (E), \iota , \pi )$ と同型です。 $\overline{\iota}$と$\overline{\pi}$は、$\iota$と$\pi$から移行から商によって群準同型が導き出されます。これにより、同型、標準準同型、$\varphi$は、Γから$\Gamma /\iota (E)$までの$v_*(\mathscr{E})$、対応するから標準準同型に関連付けられます。

#### 命題 3 {#alg-viii-s16-prop-3 .statement tag=00IM}

G と $G'$ を群とし、F と $F'$ をアーベル群とします。 $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$)$,u: G'\rightarrow G$ と $v: F\rightarrow F'$ を群準同型とします。

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

$g\in G$と$f\in F$の場合。 $\tau ''=\tau '\circ u$と書きます。 $\mathscr{E}$ を F による G の $\tau$ 拡張とします。それぞれ $\varphi_u($ で表します。 $\varphi_v,\varphi '_u,\varphi '_v)$ 標準準同型対応するから $\tau \circ u$ 内線 $u^*(\mathscr{E}) ($ まで$\tau '$ 内線 $v_*(\mathscr{E})$ へ、$\tau ''$ 内線 $u^*(v_*(\mathscr{E}))$ および $v_*(u^*(\mathscr{E})))$ へ。次に、$v_*(u^*(\mathscr{E}))$ から $u^*(v_*(\mathscr{E}))$ までの $\tau ''$ の内線番号 $\varphi_v\circ \varphi_u=$ $\varphi '_u\circ \psi \circ \varphi '_v$ の一意な準同型 $\psi$ が存在します。

$\tau \circ u$ 内線 $u^*(\mathscr{E})$ (それぞれ $\tau ''$ 内線 $u^*(v_*(\mathscr{E}))$) を $(\Gamma_u, \iota_u, \pi_u)$ (それぞれ $(\Gamma '_u, \iota '_u, \pi '_u)$) で表します。 適用補題 VIII、p. 287 から $\varphi_v\circ \varphi_u$ の 2 には、図式となる群準同型 $\psi_1: \Gamma_u\rightarrow \Gamma '_u$ が存在することがわかります。

F $^{\iota_u}$ // $\Gamma_u^{\pi_u}$ // $G'$

$v\psi_1$

${F'}^{\iota'_u}$ // ${\Gamma'_u}^{\pi'_u}$ // $G'$

通勤と$\varphi '_u\circ \psi_1=\varphi_v\circ \varphi_u$。 命題 2 を $\psi_1$ に適用すると、$\psi$ の存在が続きます。逆に、$\psi '$ にも目的のプロパティがある場合、補題 2 により $\psi '\circ \varphi '_v=\psi_1$ が得られるため、$\psi '=\psi$ (命題 2) になります。

### 4. $\tau$ の類に群法則 - 拡張機能

G を群、F をアーベル群、$\tau : G\rightarrow$ Aut(F) を群準同型とします。対角線写像 $g\mapsto$ $(g, g)$ を $\delta : G\rightarrow G\times G$ で表し、$m: F\times F\rightarrow F$ 乗法準同型 $(f_1, f_2)\mapsto$ $f_1f_2$ で表します。 $f\mapsto f^{-1}$ によって与えられる $s: F\rightarrow F$ 群準同型で表します。 $\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ と $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ を G の F による拡張 $\tau$ とします。 関係があるので、

$$
m(((\tau \times \tau )\circ \delta )(g)\cdot (f_1, f_2)) =\tau (g)\cdot m(f_1, f_2)
$$

すべての $g\in G$ とすべての $f_1, f_2\in F$ について、拡大 $m_*(\delta^*(\mathscr{E}_1\times \mathscr{E}_2))$ は $\tau$ 拡張です。 $\tau$ 拡張子 $\mathscr{E}_1$ と $\mathscr{E}_2$ の積と呼び、$\mathscr{E}_1\mathscr{E}_2$ で表します。この拡大の類は、拡大 $\mathscr{E}_1$ と $\mathscr{E}_2$ の類 (VIII、p. 288、系 1 と VIII、p. 291、 系 1）。したがって、Ex$_{\tau}(G,F)$ では合成の法則が得られます。

#### 注意 {#alg-viii-s16-n4-rem-1 .statement tag=00IN}

$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ と $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ を G の F による拡張である $\tau$ とします。$\mathscr{E}_1\mathscr{E}_2= (\Gamma , \iota , \pi )$ をこれら拡大の積とします。 VIIIの例、p. 289、構成は、ファイバー積$\Gamma_1\times_G\Gamma_2$からΓへの全射群準同型を与えます。その核は、Fからの群準同型$f\mapsto (\iota_1(f), \iota_2(f)^{-1})$の像です$\Gamma_1\times_G\Gamma_2$まで。

#### 命題 4 {#alg-viii-s16-prop-4 .statement tag=00IO}

The product of $\tau$-extensions endows the set Ex$_{\tau}(G,F)$ with the structure of an abelian group. その単位元は、半自明な拡大 $\mathscr{I}_{\tau}$ の類です。 $\tau$ 拡張 $\mathscr{E}$ の類の逆数は、$s_*(\mathscr{E})$ の類です。

法則の結合性は、図式の可換性から続きます。

$$
\begin{array}{ccc}
G & \xrightarrow{\delta} & G \times G \\
\downarrow \delta & & \downarrow \operatorname{Id} \times \delta \\
G \times G & \xrightarrow{\delta \times \operatorname{Id}} & G \times G \times G
\end{array}
$$
そして
$$
\begin{array}{ccc}
F \times F \times F & \xrightarrow{m \times \operatorname{Id}} & F \times F \\
\downarrow \operatorname{Id} \times m & & \downarrow m \\
F \times F & \xrightarrow{m} & F
\end{array}
$$

and from Corollary 2 of VIII, p. 288; Corollary 2 of VIII, p. 291; and Proposition 3 of VIII, p. 292.

$\Delta : F \to F \times F$ を対角線写像 $f \mapsto (f, f)$ とします。 $\mathscr{E} = (\Gamma, \iota, \pi)$ を $\tau$ 拡張子とします。 $\tilde{\Delta} : \Gamma \to \Gamma \times_G \Gamma$ を $\gamma \mapsto (\gamma, \gamma)$ によって与えられる群準同型とします。次の図式が通勤しています:

$$
\begin{array}{ccccc}
F & \xrightarrow{\iota} & \Gamma & \xrightarrow{\pi} & G \\
\downarrow \Delta & & \downarrow \tilde{\Delta} & & \parallel \\
F \times F & \longrightarrow & \Gamma \times_G \Gamma & \longrightarrow & G.
\end{array}
$$

VIII、p. 290 の命題 2 により、$(\tau \times \tau) \circ \delta$ 拡張子 $\delta^*(\mathscr{E} \times \mathscr{E})$ は $\Delta_*(\mathscr{E})$ と同型であることがわかります。

定数準同型 $f \mapsto 1$ を $c : F \to F$ で表します。 VIII, p. 292 の例により、合成のこの法則に対して $\mathscr{I}_\tau$ が単位元であるという事実は、$\delta^*(\mathscr{E} \times \mathscr{E})$ から $\Delta_*(\mathscr{E})$ までの同型と可換式から続きます。 図式

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times c) \circ \Delta} & F \times F \\
(c \times \operatorname{Id}_F) \circ \Delta & & \downarrow \operatorname{Id}_F \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

最後の主張は可換式図式から続きます

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times s) \circ \Delta} & F \times F \\
(s \times \operatorname{Id}_F) \circ \Delta & & \downarrow c \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

$\mathscr{E}_1 = (\Gamma_1, \iota_1, \pi_1)$ と $\mathscr{E}_2 = (\Gamma_2, \iota_2, \pi_2)$ を $\tau$ 拡張子とします。 群同型 $\Gamma_1 \times \Gamma_2 \to \Gamma_2 \times \Gamma_1$ は $(\gamma_1, \gamma_2) \mapsto (\gamma_2, \gamma_1)$ 制限するから群同型 $\sigma : \Gamma_1 \times_G \Gamma_2 \to \Gamma_2 \times_G \Gamma_1$ に与えられます。 Because of 関係

$$
\sigma(\iota_1(f), \iota_2(f)^{-1}) = (\iota_2(f^{-1}), \iota_1(f^{-1})^{-1})
$$

$f\in F$、群準同型 $\sigma$ 誘導する、移行から商、射の $\tau$ の内線番号 $\mathscr{E}_1\mathscr{E}_2$ から $\mathscr{E}_2\mathscr{E}_1$ まで。したがって、合成の法則は可換です。

#### 命題 5 {#alg-viii-s16-prop-5 .statement tag=00IP}

a) G と $G'$ を群とし、F をアーベル群とします。 $\tau : G\rightarrow$ Aut(F) と $u: G'\rightarrow G$ を群準同型とします。 写像 $u^*:$ 元$_{\tau}(G,F)\rightarrow$ 元$_{\tau\circ u}(G',F)$ は群準同型です。

b) G を群、F と $F'$ をアーベル群とします。 $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$) と $v: F\rightarrow F'$ を群準同型とします。

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

$g\in G$ と $f\in F$ の場合。 写像 $v_*:$ 元$_{\tau}(G,F)\rightarrow$ 元$_{\tau'}(G,F')$ は群準同型です。

これは図式の可換性から続きます

${G'}^{\delta}$ // $G'\times G'F\times F^m$ // F

$_uu_{\times u}$ and $v_{\times v}v$

G $^{\delta}$ // $G\times GF'\times {F'}^m$ // $F'$。

### 5. コホモロジー的記述

G を群、F をアーベル群、$\tau : G\rightarrow$ Aut(F) を群準同型とします。 $g\in G$ と $f\in F$ の場合、$\tau (g)\cdot f$ には $^gf$ も書きます。 F に値を含む G の 2 共循環は写像 $c: G\times G\rightarrow F$ であるため、$(g_1, g_2, g_3)\in G\times G\times G$ ごとに、

$$
g_{_1}c(g_2, g_3)c(g_1, g_2g_3) =c(g_1, g_2)c(g_1g_2, g_3) \tag{7}
$$

F は可換であるため、2 共サイクルの集合は、$G\times G$ から F までの写像の群の部分群です。それを$Z^2(G,F)$で表します。 G から F までの写像の群を $C^1(G,F)$ で表します。 $h\in C^1(G,F)$ と $(g_1, g_2)\in G\times G$ ごとに、集合

$$
(\partial h)(g_1, g_2) =^{g_1}h(g_2)h(g_1g_2)^{-1}h(g_1) \tag{8}
$$

単純な計算では、写像 $\partial h: G\times G\rightarrow F$ が 2 共サイクルであることがわかります。 写像 $\partial : C^1(G,F)\rightarrow Z^2(G,F)$ は群準同型です。任意の $h\in C^1(G,F)$ について、2 共環 $\partial h$ は 2 共境界と呼ばれます。 群 $Z^2(G,F)/\partial (C^1(G,F))$ は $H^2(G,F)$ で示され、F の係数とともに G の 2 番目のコホモロジー群と呼ばれます。

$*$上記記法は、群コホモロジーに関するX, §6、n$^o8$、p. 112と一致します。$*$

$\mathscr{E}= (\Gamma , \iota , \pi )$ を $\tau$ 拡張子とします。 $\sigma$ を全射法写像 $\pi ($集合理論, II, §3, No. 8, p. 86) の切断とします。つまり、G から Γ までの写像で、すべてについて $\pi (\sigma (g)) =g$ が成り立ちます。 G の $g$。各 $g_1, g_2\in G$、$\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}$ 属するから Ker($\pi$ ) に対して、次のような一意な写像 $c_{\sigma}: G\times G\rightarrow F$ が存在します。

$$
\iota (c_{\sigma}(g_1, g_2)) =\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1} \tag{9}
$$

すべての$g_1, g_2\in G$に。 $\sigma$ が群準同型である場合に限り、写像 $c_{\sigma}$ は値 1 で定数になります。

#### 命題 6 {#alg-viii-s16-prop-6 .statement tag=00IQ}

写像 $c_{\sigma}$ は群 $Z^2(G,F)$ の元であり、コホモロジー群 $H^2(G,F)$ の類は、$\tau$ 拡張子 $\mathscr{E}$ の類にのみ依存します。

写像 $c_{\sigma}$ は $\sigma$ に関連付けられた 2 共循環であり、$H^2(G,F)$ のコホモロジー 類は $\tau$ の拡張 $\mathscr{E}$ のコホモロジー 類であると言います。

まず、$c_{\sigma}$ が共循環条件を満たすことを確認しましょう。 $g_1,g_2$、$g_3$ を G の元とします。VIII、p. 285、および (9) の公式 (1) を使用すると、関係が得られます。

$$
\iota (^{g_1}c_{\sigma}(g_2, g_3)c_{\sigma}(g_1, g_2g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_2g_3)^{-1}\sigma (g_1)^{-1}\sigma (g_1)\sigma (g_2g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

そして

$$
\iota (c_{\sigma}(g_1, g_2)c_{\sigma}(g_1g_2, g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}\sigma (g_1g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

したがって、写像 $c_{\sigma}$ は、$Z^2(G,F)$ の元です。

ここで、$H^2(G,F)$ の $c_{\sigma}$ の像が、選択された切断 $\sigma$ から独立していることを証明しましょう。 $\sigma$ と $\sigma '$ をそのような切断とします。 G のすべての元 $g$ に対して、$\sigma '(g) =\iota (a_g)\sigma (g)$ となる F の一意元 $a_g$ が存在します。 $g_1$ と $g_2$ を G の元とします。 定義 (9) を使用すると、次の等式が得られます。

$$
\iota (c_{\sigma'}(g_1, g_2)) =\sigma '(g_1)\sigma '(g_2)\sigma '(g_1g_2)^{-1}
$$

$$
=\iota (a_{g_1})\sigma (g_1)\iota (a_{g_2})\sigma (g_2)\sigma (g_1g_2)^{-1}\iota (a_{g_1g_2})^{-1} \tag{10}
$$

$$
=\iota (a_{g_1})\iota (^{g_1}a_{g_2})\iota (c_{\sigma}(g_1, g_2))\iota (a_{g_1g_2})^{-1}
$$

群 F は可換なので、関係となります。

$$
c_{\sigma'}(g_1, g_2)c_{\sigma}(g_1, g_2)^{-1}= (^{g_1}a_{g_2})a^{-1}_{g_1g_2}a_{g_1}= (\partial a)(g_1, g_2) \tag{11}
$$

(8)より次のようになります。これにより、$H^2(G,F)$ 一致するの $c_{\sigma'}$ と $c_{\sigma}$ の類が証明されます。

最後に、$\mathscr{E}= (\Gamma , \iota , \pi )$ と $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ を同型 $\tau$ 拡張子とし、$u:\mathscr{E}\rightarrow \mathscr{E}'$ を $\tau$ 拡張子の射とし、$\sigma$ を写像 $\pi$ の切断とします。 写像 $u\circ \sigma$ は写像 $\pi '$ の切断で、$c_{\sigma}=c_{u\circ\sigma}$ があります。したがって、$H^2(G,F)$の$c_{\sigma}$の類は、Ex$_{\tau}(G,F)$の$\mathscr{E}$の類のみに依存します。

$\Theta_{\tau}$ : Ex$_{\tau}(G,F)\rightarrow H^2(G,F)$、またはより単純に $\tau$ 拡張 $(\Gamma , \iota , \pi )$ の類を 2 共サイクル $c_{\sigma}$ の類に送信する Θ、写像で表します。ここで、$\sigma$ は射影$\pi$の切断。

#### 定理 1 {#alg-viii-s16-thm-1 .statement tag=00IR}

写像 Θ は Ex$_{\tau}(G,F)$ から $H^2(G,F)$ までの群同型です。

まずΘが群準同型であることを証明しましょう。 $\mathscr{E}= (\Gamma , \iota , \pi )$ と $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ を $\tau$ 拡張子とし、$\sigma$ (それぞれ $\sigma '$) を写像 $\pi$ (それぞれ $\pi '$) の切断とします。 $\tau$ 拡張子 $\mathscr{E}$ と $\mathscr{E}'$ の $\mathscr{E} \mathscr{E}'= (\Gamma '', \iota '', \pi '')$ 積で表します。 VIIIの注意、p. 293から全射準同型で元の$\Gamma ''$、$\Gamma \times_G\Gamma '$の$(\gamma , \gamma ')$を$[\gamma , \gamma ']$像で表します。 元 $g$ を $[\sigma (g), \sigma '(g)]$ に送信する G から $\Gamma ''$ への写像は、写像 $\pi ''$ の切断 $\sigma ''$ です。 $g_1$ と $g_2$ を G の元とします。関係となります。

$$
\iota ''(c_{\sigma''}(g_1, g_2)) =\sigma ''(g_1)\sigma ''(g_2)\sigma ''(g_1g_2)^{-1}
$$

$$
= [\iota (c_{\sigma}(g_1, g_2)), \iota '(c_{\sigma'}(g_1, g_2)]
$$

$$
=\iota ''(c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2))
$$

したがって、$c_{\sigma''}(g_1, g_2) =c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2)$ となります。

写像 Θ が単射であることを証明しましょう。 $\mathscr{E}= (\Gamma , \iota , \pi )$ を $\tau$ 拡張とし、$\sigma$ を写像 $\pi$ の切断とし、$H^2(G,F)$ の $c_{\sigma}$ の像が自明であるようにします。次のような写像 $a: G\rightarrow F$ が存在します。

$$
c_{\sigma}(g_1, g_2) = (^{g_1}a(g_2))a(g_1g_2)^{-1}a(g_1)
$$

すべての$g_1, g_2\in G$に。その後、定義する $\sigma ': G\rightarrow \Gamma$ によって

$$
\sigma '(g) =\iota (a(g)^{-1})\sigma (g)
$$

$g\in G$の場合。 (11) を使用すると、$c_{\sigma'}$ は値 1 で定数であることがわかります。従って、$\sigma '$ は群準同型となり、$\tau$ 拡張 $\mathscr{E}$ が半自明であることが証明されます (I, §6, No. 1, p. 67, 命題 4)。

写像 Θ が全射であることを証明しましょう。 $c$を$Z^2(G,F)$の元とします。 集合 $\Gamma  = F\times G$ に次の法則または合成を与えます: (12) $(f_1, g_1)(f_2, g_2) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)$

$f_1, f_2\in F$ と $g_1, g_2\in G$ のすべてに。 関係があります

$$
(f_1, g_1) ((f_2, g_2)(f_3, g_3)) = (f_1, g_1)(f_2(^{g_2}f_3)c(g_2, g_3), g_2g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)(^{g_1}c(g_2, g_3))c(g_1, g_2g_3), g_1g_2g_3)
$$

そして

$$
((f_1, g_1)(f_2, g_2)) (f_3, g_3) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)(f_3, g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)c(g_1, g_2)c(g_1g_2, g_3), g_1g_2g_3)
$$

$f_1, f_2, f_3\in F$ と $g_1,g_2, g_3\in G$ 全員に。 $c$ は 2 共循環であるため、この法則は結合的であることがわかります。 $(f, g)\in \Gamma$ ごとに、

$$
(f, g)(c(e, e)^{-1}, e) = (f(^gc(e, e)^{-1})c(g, e), g)
$$

さて、2 共サイクルの定義から $c(g, e) =^gc(e, e)$ が得られ、そこから $(f, g)(c(e, e)^{-1}, e) = (f, g)$ が推定されます。同様に証明します

$$
(c(e, e)^{-1}, e)(f, g) = (f c(e, e)^{-1}c(e, g), g) = (f, g)
$$

従って、(12) で定義された合成の法則は単位元 $(c(e, e)^{-1}, e)$ を持ち、Γ のすべての元 $(f, g)$ は可逆であり、その逆数は

$$
(^{g^{-1}}(f^{-1}c(e, e)^{-1}c(g, g^{-1})^{-1}), g^{-1})
$$

従って、Γに群構造を与えました。 $f$ を $(c(e, e)^{-1}f, e)$ に送信する$\iota : F\rightarrow G$ 写像を $\pi : \Gamma \rightarrow G$ で 2 番目の射影を、$\sigma$ 写像 $g\mapsto (1, g)$ で表します。 写像 $\iota$ と $\pi$ は群準同型であるため、トリプル $\mathscr{E}= (\Gamma , \iota , \pi )$ は $\tau$ 拡張、$\sigma$ は写像 $\pi$ の切断、および関連するコサイクルです。 $c_{\sigma}$ は $c$ に等しいため、

$$
\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}= (1, g_1)(1, g_2)(1, g_1g_2)^{-1}= (c(g_1, g_2), g_1g_2)(1, g_1g_2)^{-1}
$$

$$
= (c(g_1, g_2)c(e, g_1g_2)^{-1}, e) = (c(e, e)^{-1}c(g_1, g_2), e)
$$

$g_1, g_2\in G$の場合。

#### 注意 {#alg-viii-s16-n5-rem-1 .statement tag=00RK}

G を群、F と $F'$ をアーベル群、$\tau$ (それぞれ $\tau '$) を G から F の自己同型群 (それぞれ $F'$) までの群準同型とします。 $v: F\rightarrow F'$ は群射になる

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{13}
$$

$g\in G$ と $f\in F$ 用。 $\alpha$をEx$_{\tau}(G,F)$の元とします。共環 $c$ が $\Theta (\alpha )$ を表す場合、$v\circ c$ は $\Theta (v_*(\alpha ))\in H^2(G,F')$ を表します。

### 6. 制限とコア制限

Gと$G'$を群、Fをアーベル群、$\tau$をGからFの自己同型群までの準同型とします。$u: G'\rightarrow G$を群準同型とします。 $\tau '=\tau \circ u$と書きます。

$\psi : G\times G\rightarrow F$ が F に値をもつ G の 2 共環である場合、$(g_1, g_2)\mapsto \psi (u(g_1), u(g_2))$ で与えられる $G'\times G'$ から F までの写像 $\psi \circ (u\times u)$ は、F に値をもつ $G'$ の 2 共環であり、写像 $\psi \mapsto \psi \circ (u\times u)$ $Z^2(G,F)$ から $Z^2(G',F)$ 誘導する群準同型 $u^*: H^2(G,F)\rightarrow H^2(G',F)$ まで。任意の $\lambda \in H^2(G,F)$ について、元 $u^*(\lambda )$ は、$u$ によって $\lambda$ の逆像と呼ばれます。 $G'$ が G の部分群で、$u: G'\rightarrow G$ が標準単射のとき、準同型 $u^*$ は G から $G'$ まで制限準同型と呼ばれます。これを Res$^G_{G'}$ で表します。 Gが$G'$の商、$u: G'\rightarrow G$が標準全射のとき、準同型$u^*$はGから$G'$までインフレーション準同型と呼ばれます。

#### 命題 7 {#alg-viii-s16-prop-7 .statement tag=00IS}

上からの記法では、次の図式が通勤します。

例$_{\tau}(G,F)^{u^*}$ // 例$_{\tau}(G',F)$

$\Theta_{\tau}\Theta_{\tau'}$

$H_2(G,F)^{u^*}$ // $H_2(G',F)$。

H を有限添字の G の部分群とします。 $s$ を G から $H\backslash G$ までの標準全射の切断とします。 乗法によってそれ自身上の G の右作用によって誘発される $H\backslash G$ 上の G の $(g, x)\mapsto x\cdot g$ 右作用で表します。すべての $x\in H\backslash G$ と $g\in G$ について、元 $s(x)gs(x\cdot g)^{-1}$ 属するが H に変換されることに注意してください。したがって、任意の写像 $c: H\times H\rightarrow F$ について、関係までに定義する写像 $\widetilde{c}_s: G\times G\rightarrow F$ を求めることができます。

$$
\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$g_1,g_2\in G$の場合。 写像 $c\mapsto \widetilde{c}_s$ は、$F^{H\times H}$ から $F^{G\times G}$ までの群準同型です。

#### 補題 4 {#alg-viii-s16-lem-4 .statement tag=00IT}

$c: H\times H\rightarrow F$ が F に値をもつ H の 2 共環である場合、$\widetilde{c}_s$ は F に値をもつ G の 2 共環です。

$g_1,g_2$ と $g_3$ を G の元とします。すべての $i\in  \{1,2,3\}$ に対して、関係により定義する写像 $h_i: H\backslash G\rightarrow H$ となります。

$$
h_i(x) =s(x\cdot g_1\cdots g_{i-1})g_is(x\cdot g_1\cdots g_i)^{-1}
$$

$x\in H\backslash G$の場合。ご了承ください

$$
h_1(x)h_2(x) =s(x)g_1g_2s(x\cdot g_1g_2)^{-1}
$$

$$
h_2(x)h_3(x) =s(x\cdot g_1)g_2g_3s(x\cdot g_1g_2g_3)^{-1}
$$

$x\in H\backslash G$の場合。そうすると関係になります

$$
^{g_1}\widetilde{c}_s(g_2, g_3)\widetilde{c}_s(g_1g_2, g_3)^{-1}\widetilde{c}_s(g_1, g_2g_3)\widetilde{c}_s(g_1, g_2)^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(s(x)g_2s(x\cdot g_2)^{-1}, s(x\cdot g_2)g_3s(x\cdot g_2g_3)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h_1(x)h_2(x), h_3(x))^{-1}
$$

$$
\times c(h_1(x), h_2(x)h_3(x))c(h_1(x), h_2(x))^{-1})
$$

$$
=\prod_{x\in H\backslash G}^{s(x\cdot g_1^{-1})^{-1}h_1(x\cdot g^{-1}_1)}c(h_2(x\cdot g_1^{-1}), h_3(x\cdot g_1^{-1}))
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}h_1(x)}c(h_2(x), h_3(x))^{-1}
$$

$$
= 1
$$

ここで、2 番目の等式は、$c$ が 2-cocycle であるという事実から導かれます。

#### 補題 5 {#alg-viii-s16-lem-5 .statement tag=00IU}

$c$ が 2 共有境界である場合、$\widetilde{c}_s$ も同様です。

$t: H\rightarrow F$ を写像とし、$c=\partial t$ とします。 $\widetilde{t}_s: G\rightarrow F$ を写像として定義します。

$$
\widetilde{t}_s(g) =\prod_{x\in H\backslash G}^{s(x)^{-1}}t(s(x)gs(x\cdot g)^{-1})
$$

$g\in G$の場合。 関係 $\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}s(x)g_1s(x\cdot g_1)^{-1}}t(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$ から続く $\widetilde{c}_s=\partial \widetilde{t}_s$ を証明すれば十分です

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(t(s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}t(s(x)g_1s(x\cdot g_1)^{-1}))
$$

$$
=\partial \widetilde{t}_s(g_1, g_2)
$$

$g_1, g_2\in G$用。

#### 補題 6 {#alg-viii-s16-lem-6 .statement tag=00IV}

$c$ を F の値を持つ H の 2 共環とします。 群 $H^2(G,F)$ の $\widetilde{c}_s$ の像は、切断 $s$ の選択に依存しません。

$s'$をGから$H\backslash G$までの標準全射の切断とします。 $h: H\backslash G\rightarrow H$ を関係によって特徴づけられる写像とします

$$
s'(x) =h(x)s(x)
$$

$x\in H\backslash G$の場合。 2 共サイクル $\widetilde{c}_{s'}$ は関係によって与えられます。

$$
\widetilde{c}_{s'}(g_1, g_2)
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}h(x)^{-1}}c(h(x)s(x)g_1s'(x\cdot g_1)^{-1}, s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}(-1''-1-1$

$$
\times \prod_{x\in H\backslash G}c(h(x), s(x)g_1g_2s(x\cdot g_1g_2))
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

$=\prod_{x\in H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c(h(x\cdot g_1)^{-1}, h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}-1-1-1$

$\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(h(x)^{-1}, s'(x)g_1g_2s'(x\cdot g_1g_2)^{-1})^{-1}
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

$=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1})$

$s(x)^{-1}-1-1-1$

$\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$ $\times \prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(h(x)^{-1}, h(x)s(x)g_2s'(x\cdot g_2)^{-1})$

$s(x)^{-1}(-1''-1-1$

$$
\times \prod_{x\in H\backslash G}c(h(x), s(x)g_1g_2s(x\cdot g_1g_2))
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

$g_1, g_2\in G$ 全員のために。最初の等式は、コサイクル関係 (VIII, p. 295, 公式 (7)) を元に適用したものです。

$h(x)^{-1},h(x)s(x)g_1s'(x\cdot g_1)^{-1}$、および$s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$;

2 番目は適用コサイクル関係から元によって取得されます。

$s(x)g_1s(x\cdot g_1)^{-1},h(x\cdot g_1)^{-1}$、および$h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$;最後は、写像 $x\mapsto x\cdot g_1$ が $H\backslash G$ の置換であるという事実を単純に使用しています。

得られた式対応するの最後の 2 行を 2 共有境界にします。 $\widetilde{c}_{s'}$ は、$(g_1, g_2)\in G^2$ の値が次の式で与えられるコサイクルと同じ $H^2(G,F)$ の類を持つことがわかります。

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}h(x\cdot g_1g_2)^{-1})
$$

$s(x)^{-1}-1-1-1$

$$
\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))
$$

$=\prod_{x\in H\backslash G}^{g_1s(x\cdot g_1)^{-1}}c(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})^{-1}$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})
$$

$-1-1-1)$

$\times c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$ $=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

$gs(x)^{-1}-1-1-1$

$$
\times \prod_{x\in H\backslash G^1}c(s(x)g_2s(x\cdot g_2), h(x\cdot g_2))
$$

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(c(s(x)g_1g_2s(x\cdot g_1g_2)^{-1}, h(x\cdot g_1g_2)^{-1})
$$

$$
\times c(s(x)g_1s(x\cdot g_1)^{-1}, h(x\cdot g_1)^{-1})^{-1})
$$

ここで、最初の等式はコサイクル関係から元に適用されます。

$s(x)g_1s(x\cdot g_1)^{-1},s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$、および$h(x\cdot g_1g_2)^{-1}$。

得られた式対応するの最後の 2 行を 2 共有境界にします。 $\widetilde{c}_{s'}$ 一致するの類が $\widetilde{c}_s$ のそれと一致することがわかります。

群 $H^2(H,F)$ から群 $H^2(G,F)$ までの準同型を構築しました。これを H から G までコアストリクション準同型と呼び、Cor$^G_H$ で表します。

#### 命題 8 {#alg-viii-s16-prop-8 .statement tag=00IW}

H を有限添字の G の部分群とします。 自己準同型 Cor$^G_H\circ$ Res$^G_H$ の群 $H^2(G,F)$ 一致すると乗法 by 添字 (G : H)。

$\alpha$ を $H^2(G,F)$ の元とし、$c$ を $\alpha$ を表す $Z^2(G,F)$ の元とします。 元 Cor$^G_H\circ$ Res$^G_H(\alpha )$ は、$(g_1, g_2)\in G^2$ の値が次の式で与えられる共環の類です。

$$
\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
=\prod_{x\in H\backslash G}c(g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1}))
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1}))
$$

$=\prod_{x\in H\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}$

$$
\times \prod_{x\in H\backslash G}^{g_1}c(s(x)^{-1}, s(x)g_2s(xg_2)^{-1})
$$

$$
\times \prod_{x\in H\backslash G}(c(s(x)^{-1}, s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}c(s(x)^{-1}, s(x)g_1s(x\cdot g_1)^{-1}))
$$

最初の等式は、元に適用されたコサイクル関係 (VIII、p. 295、公式 (7)) から来ています。

$s(x)^{-1},s(x)g_1s(x\cdot g_1)^{-1}$、および$s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$;

2 番目は適用コサイクル関係から元によって取得されます

$g_1,s(x\cdot g_1)^{-1}$、および$s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$。

コバウンダリー を削除すると、Cor$^G_H\circ$ Res$^G_H(\alpha )$ が、$(g_1, g_2)\in G^2$ の値が次の式で与えられる共環の類であることがわかります。

$$
\prod_{x\in H\backslash G}c(g_1, g_2s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x\cdot g_1g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, g_2)
$$

$$
\times \prod_{x\in H\backslash G}c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
=\prod_{x\in H\backslash G}^{g_1}c(g_2, s(x\cdot g_2)^{-1})^{-1}c(g_1g_2, s(x\cdot g_1g_2)^{-1})c(g_1, s(x\cdot g_1)^{-1})^{-1}
$$

$$
\times c(g_1, g_2)^{(G:H)}
$$

それが結果を証明しています。

### 7. ガロア代数

Kを可換体とします。 E が K-代数の場合、その自己同型群を Aut$_K(E)$ で表します。 E が体 K のガロア拡大である場合、群 Aut$_K(E)$ は単純にガロア群 Gal(E$/K$) (V, §10, No. 2, p. 58) です。

G を群とします。 $A (K,G)$-代数は、群準同型 $\lambda : G\rightarrow$ Aut$_K(E)$ を備えたK-代数 E です。 準同型 $\lambda$ は、E に G の演算子を持つ群の構造と、左の K[G] モジュールの構造に次の式で与えられる外部法則を与えます。

$$
((\sum_{g\in G}\mu_gg)x=\sum_{g\in G}\mu_g\lambda (g).x \tag{14}
$$

K[G] のすべての $x\in L$ とすべての元 $(\mu_g)_{g\in G}$ に対して。 $(K,G)$代数の射は代数の射であり、演算子を使用すると群の射でもあります。

$(K$、G)-代数、積 K-代数 $\prod_{i\in I}E_i$ のすべての族 $(E_i)_{i\in I}$ に対して、積群の構造に演算子が与えられたものは、$(K$、G)-代数です。

E が $(K$, G)-代数である場合、G のもとでの不変量 E の元の集合 $E^G$ は E の部分代数です。

E を $(K$, G)-代数とし、G は $\lambda : G\rightarrow$ Aut$_K(E)$ によって作用します。 $K'$ が K の拡大である場合、任意の $g\in G$ について、$\lambda '(g)$ を $K'$-代数 $L_{(K')}$ の自己同型 ID$_{K'}\otimes \lambda (g)$ とします。次に、$\lambda ':g\mapsto \lambda '(g)$ は $L_{(K')}$ に $(K'$、G)-代数の構造を与えます。

群 H と H セット X および Y が与えられると、X から Y までの H セットの射のうち $\mathscr{F}_H(X,Y)$ 集合で表されます。 $h\in H$ と $x\in X$ ごとに $f(hx) =hf(x)$ となる、写像 $f: X\rightarrow Y$ の集合です。

G を単位元 $e$ を伴う群とし、H を G の部分群とし、E を $(K$、H)-代数とする。 H から G への共帰によって E から推定される $(K,G)$-代数は、Coind$^G_H$(E) で示され、G から準同型 $\lambda$ によって与えられる G の作用を備えた K-代数 $\mathscr{F}_H(G,E)$ です。 Aut$_K$(Coind$^G_H(E)$) によって定義されました

$$
(\lambda (g)\cdot f)(g') =f(g'g) \tag{15}
$$

$f\in$ コイン$^G_H(E)$ と $g, g'\in G$ の場合。

#### 補題 7 {#alg-viii-s16-lem-7 .statement tag=00IX}

a) S を G の部分集合とし、G のすべての元を $h\in H$ と $s\in S$ を使用して $hs$ として一意に記述できるようにします。 Then the mapping that sends $f$ to $(f(s))_{s\in S}$ is an isomorphism from the K-algebra Coind$^G_H(E)$ to the K-algebra $\mathscr{F}(S,E)$ of mappings from S to E.

b) E が K に対して有限次数を持ち、G の H の添字が有限である場合に限り、代数 Coind$^G_H(E)$ は K に対して有限次数を持ちます。この場合、公式となります。

[コイン$^G_H(E) : K] = (G : H)[E : K]$。

c) $E^H$ を、E の群 H および Coind$^G_H(E)^G$ の Coind$^G_H(E)$ の群 G の不変量の代数とします。コイン$^G_H(E)$からEまで写像$f\mapsto f(e)$、コイン$^G_H(E)^G$から$E^H$まで制限するから代数同型。

主張 a) は定義から続き、b) を暗示します。 (15) により、G から E への写像は、H の下で E の不変量である値元と定数である場合に限り、G の下で Coind$^G_H(E)$ の元不変量となります。

#### 注意 1 {#alg-viii-s16-n7-rem-1 .statement tag=00IY}

G を群、G の H 部分群、H の N 部分群とします。E を $(K$、N)-代数とします。 $\alpha$を$\mathscr{F}_H(G,\mathscr{F}_N(H,E))$の元とします。 関係あります

$$
\alpha (g)(nh) =n(\alpha (g)(h)) \tag{16}
$$

$g\in G,h\in H$、$n\in N$、関係ごとに

$$
\alpha (hg)(h') = (h\alpha (g))(h') =\alpha (g)(h'h) \tag{17}
$$

すべての $h, h'\in H$ とすべての $g\in G$ に対して。従って、$g\in G$ と $n\in N$ ごとに $\alpha (ng)(e) =\alpha (g)(n) =$ $n(\alpha (g)(e))$ となります。従って、写像を検討できます。

$$
\psi :\mathscr{F}_H(G,\mathscr{F}_N(H,E))\rightarrow \mathscr{F}_N(G,E)
$$

$\mathscr{F}_H(G,\mathscr{F}_N(H,E))$ の $\alpha$ と G の $g$ に対して関係 $\psi (\alpha )(g) =\alpha (g)(e)$ によって定義されます。 写像 $\psi$ は Coind$^G_H$(Coind$^H_N(E)$) から Coind$^G_N(E)$ までの代数同型であり、その逆は元 $\beta$ を $\mathscr{F}_N(G,E)$ から写像 $\alpha$ に送信します。 $g\in G$ と $h\in H$ の場合は関係 $\alpha (g)(h) =\beta (hg)$ です。

ここで、有限群 G と、G から Aut$_K(L)$ への準同型 $\lambda$ によって与えられる G の作用が付与された有限次数の縮小 (V, §6, No. 6, p. 32) 可換K-代数 L を仮定します。 $x\in L$ と $g\in G$ については、L の自己同型 $\lambda (g)$ の下に $x$ の $g\cdot x$ 変換で表します。 $\mathscr{S}$ を最大理想 L の集合とします。 自己同型 $\lambda (g)$ の L の下の $g\cdot \mathfrak{m}$ 変換の元 $\mathfrak{m}$ の $\mathscr{S}$ で表します。 $\mathscr{S}$の元です。 $\mathscr{S}$ のすべての $\mathfrak{m}$ に対して、体 $L/\mathfrak{m}$ は K の有限拡大です。 射影を $\pi_{\mathfrak{m}}: L\rightarrow L/\mathfrak{m}$ と書き、G の $\mathfrak{m}$ の $G_{\mathfrak{m}}$ 固定群、つまり $g\cdot \mathfrak{m}=\mathfrak{m}$ のような $g\in G$ の集合で表します。 The K-algebra $L/\mathfrak{m}$ is endowed with an action of $G_{\mathfrak{m}}$ through the homomorphism $\lambda_{\mathfrak{m}}$ from $G_{\mathfrak{m}}$ to Aut$_K(L/\mathfrak{m})$ that sends an element $h$ of $G_{\mathfrak{m}}$ to the automorphism of $L/\mathfrak{m}$ deduced from $\lambda (h)$ when passing to the quotients.

$\mathscr{O}$ を $\mathscr{S}$ の G の軌道の集合とします。 軌道 $\sigma \in \mathscr{O}$、集合 $\mathfrak{a}_{\sigma}=\bigcap_{\mathfrak{m}\in\sigma}\mathfrak{m}$、$L_{\sigma}= L/\mathfrak{a}_{\sigma}$ が与えられます。 $\mathfrak{a}_{\sigma}$ は G の下で不変なので、移行から商までに、G の作用が L 定義する準同型 $\lambda_{\sigma}$ G から Aut$_K(L_{\sigma})$ までとなります。最後に、Lから$L_{\sigma}$までを$\pi_{\sigma}$ 標準写像と表します。

#### 補題 8 {#alg-viii-s16-lem-8 .statement tag=00RL}

a) $g\in G,\sigma \in \mathscr{O}$ および $\mathfrak{m}\in \sigma$ ごとに、

$[L_{\sigma}: K] =$ カード($\sigma$ )$[L/\mathfrak{m}: K]$。

b) 写像 $\pi :x\mapsto (\pi_{\sigma}(x))_{\sigma\in\mathscr{O}}$ は、L から $\prod_{\sigma\in\mathscr{O}}L_{\sigma}$ までの $(K,G)$-代数の同型です。

c) それぞれ$L^G($で表します。 L の $L^G_{\sigma})$ 部分代数 (それぞれ $L_{\sigma}$) の元は G の作用の下で不変です。次に、$L^G$ から $\prod_{\sigma\in\mathscr{O}}L^G_{\sigma}$ までの $\pi$ 誘導する同型です。

代数 L が減少し、有限次数、L の最大理想の共通部分が 0 に減少します (VIII、p. 173、系 2)。 さらに、$\mathfrak{m}$ と $\mathfrak{m}'$ が L の 2 つの異なる最大理想である場合、$\mathfrak{m}+\mathfrak{m}'= L$ が得られます。 I, §8, No. 11、p. 110、標準写像のLから$\prod_{\mathfrak{m}\in\mathscr{S}}L/\mathfrak{m}$までの命題10は同型となり、$L/\mathfrak{a}_{\sigma}$から$\prod_{\mathfrak{m}\in\sigma}L/\mathfrak{m}$までは$\sigma \in \mathscr{O}$ごとに標準写像になります。 主張 a) が続きます。 $\mathscr{O}$ は $\mathscr{S}$ の分割であるため、主張 b) が続きます。 主張 c) は b) の明らか帰結です。

$\sigma$ の軌道 $\sigma \in \mathscr{O}$ と元 $\mathfrak{m}$ を修正しましょう。 集合 $F_{\mathfrak{m}}$ = コイン$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$、$F_{\mathfrak{m}}$ の G の $\lambda_{F_{\mathfrak{m}}}$ 作用で表します。 任意の $x\in L$ について、$g$ を $\pi_{\mathfrak{m}}(gx)$ に送信する G から $L/\mathfrak{m}$ までの $\overline{x}$ 写像で表します。 By formula (15) of VIII, p. 305 and the definition of the action of $G_{\mathfrak{m}}$ on $L/\mathfrak{m}$, it is immediate that $\overline{x}$ belongs to $F_{\mathfrak{m}}$, and the mapping $u:x\mapsto \overline{x}$ from L to $F_{\mathfrak{m}}$ satisfies $\lambda_{F_{\mathfrak{m}}}(g)\circ u=u\circ \lambda (g)$ for $g\in G$. 他の語、$u$は$(K$、G)-代数の射です。

#### 補題 9 {#alg-viii-s16-lem-9 .statement tag=00IZ}

射 $u$ は核 $\mathfrak{a}_{\sigma}$ と全射です。 $u$ から移行から商によって導出された写像は、$L_{\sigma}$ から $F_{\mathfrak{m}}$ までの $(K,G)$-代数の同型です。

$\pi_{\mathfrak{m}}$の核は$\mathfrak{m}$に等しいため、$u$の⟦9​​⟧は$\bigcap_{g\in G}g^{-1}.\mathfrak{m}=\mathfrak{a}_{\sigma}$に等しい。 $u$ が全射であることを証明するには、ベクトル空間 $L_{\sigma}=$ $L/\mathfrak{a}_{\sigma}$ と $F_{\mathfrak{m}}$ が K に対して同じ次元を持つことを証明すれば十分です。 さて、すべてのイデアル $g\cdot \mathfrak{m}$ は L で同じ次元を持ち、次のようになります。 補題 8、a)、

$[L_{\sigma}: K] =$ カード($\sigma$ )$.[L/\mathfrak{m}: K]$。

さらに、補題 7、b) までに、

$$
[F_{\mathfrak{m}}: K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]
$$

Card($\sigma$ ) $= (G : G_{\mathfrak{m}})$ があるので、等式 $[L_{\sigma}: K] =$ $[F_{\mathfrak{m}}: K]$ を証明しました。

さらに、G から Aut$_K(L)$ までの準同型 $\lambda$ が単射であると仮定します。私たちは同一視する K で、その像は L から写像 $\xi \mapsto \xi \cdot 1$ までです。 Ω を K の代数閉拡大とします。共誘起 $(\Omega$, G)-代数 Coind$^G_{\{e\}}(\Omega )$ を使用して、G から Ω 一致するまで写像の集合 $\mathscr{F}(G,\Omega )$ とします。これは、階数 1 のフリー Ω[G] モジュールです。$\mathscr{H}$ を、L から Ω までの K-代数準同型の集合とします。私たちは $\mathscr{H}$ までに $(g, \chi )\mapsto \chi \circ \lambda (g)$ に G の定義する右作用です。次に、Ω代数 $\mathscr{F}(\mathscr{H},\Omega )$ には、$\mathscr{H}$ 上の G の右作用から推定される $(\Omega$, G)-代数の構造が与えられます。

#### 補題 10 {#alg-viii-s16-lem-10 .statement tag=00J0}

L を K 上のエタールである $(K,G)$-代数とする。写像 $\psi$ $L_{(\Omega )}$ から $\mathscr{F}(\mathscr{H},\Omega )$ は関係によって特徴付けられる

$$
\psi (\xi \otimes x) = (\xi \chi (x))_{\chi\in\mathscr{H}}
$$

は、$(K,G)$-代数の同型です。

L はエタールなので、写像 $\psi$ はΩ代数 (V, §6, No. 3, p. 30, 命題 2 と V, §6, No. 3, p. 29, 命題) の同型です。 1、c))。 関係があります

$\psi$((ID $\otimes \lambda (g)$)$(\xi \otimes x)$) $= (\xi (\chi \circ \lambda (g))(x))_{\chi\in\mathscr{H}}$

$\xi \in \Omega ,x\in L$と$g\in G$の場合。したがって、$\psi$ は、G)-代数の $(\Omega$ の射です。

#### 定理 2 {#alg-viii-s16-thm-2 .statement tag=00J1}

Gを有限群とし、LをGからAut$_K(L)$への単射準同型$\lambda$によって与えられるGの作用を与えられた有限次数の可換K-代数とする。したがって、次のプロパティは同等になります。

(i) G の部分群 H、有限次数の K のガロア拡大 E、H から Gal(E$/K$) までの同型、および L から $(K,G)$ 代数の同型が存在します。コイン$^G_H(E)$。

(ii) 代数 L はエタール、$\mathscr{H}$ は同次主 G セット (I, §5, No. 6、p. 60、定義 7) です。

(iii) $(\Omega ,G)$-代数 $\psi : L_{(\Omega )}\rightarrow \mathscr{F}(G,\Omega )$ の同型が存在します。他の語では、$g\in G$ ごとに、$\Omega^G$ の自己同型 $\psi \circ \lambda (g)_{(\Omega )}\circ \psi^{-1}$ は自己同型に等しい

$$
(x_h)_{h\in G}\longmapsto (x_{hg})_{h\in G}
$$

(iv) 代数 L は削減され、L は階数 1 の空き K[G] モジュールです。

(v) 代数 L は約定され、Card(G) = [L : K] があり、K は G の作用の下で不変である元の L の部分環です。

(vi) 代数 L が還元され、群 G は L の最大イデアルの集合に推移的に作用し、L のすべての最大イデアル $\mathfrak{m}$、固定群 $G_{\mathfrak{m}}$ に対して推移的に作用します。 G の $\mathfrak{m}$ は、$L/\mathfrak{m}$ に忠実に作用し、K を不変量の部分体として認めます。

(i)$\Rightarrow$(ii):HからAut$_K(E)$までの有限次数と$\tau$同型のKのガロア拡大をEとします。 S を H を法とする G の右剰余類の代表の系とします。 K-代数 F = Coind$^G_H(E)$ は $\mathscr{F}(S,E)$ (補題 7, a)) と同型です。したがって、それはエターレです。 F 上の G の$\lambda_F$ 作用と表します。さらに、$\psi$ を E から Ω まで K-代数準同型とし、$\chi_0$ を F から Ω まで準同型 $f\mapsto \psi (f(e))$ とします。 $g\in G$ を $\chi_0\circ \lambda_F(g) =\chi_0$ となるようにします。 $\psi$ は単射なので、$f\in F$ ごとに $f(g) =f(e)$ が得られます。 補題 7、a) を考慮すると、$g\in H$ があり、公式までに

$$
f(h) =\tau (h)\cdot f(e) \tag{18}
$$

これは $h\in H$ ごとに当てはまりますが、これは $g=e$ の場合にのみ発生します。一方、V, §10, No. 6、p. 66 の補題 7、b) と定理 3 により、

[F : K] = (G : H)[E : K] = (G : H) カード(H) = カード(G)。

F から Ω までの K 準同型射の集合 $\mathscr{K}$ は、F がエタール (V, §6, No. 5, p. 32, 命題 4) であるため、基数 [F : K] となり、Card($\mathscr{K}$) $=$ Card(G) となります。上記より、G の $\chi_0$ の固定群は $\{e\}$ に等しいので、$\mathscr{K}$ は同次主 G 集合です。

(ii)$\Rightarrow$(iii): L がエタール、$\mathscr{H}$ が同次主 G セットであると仮定します。 補題 10 までに、$(\Omega$、G)-代数 $L_{(\Omega )}$ と $\mathscr{F}(\mathscr{H},\Omega )$ は同型になります。 $\mathscr{H}$ は同次主 G 集合であるため、$(\Omega$、G)-代数 $\mathscr{F}(\mathscr{H},\Omega )$ および $\mathscr{F}(G,\Omega )$ は同型です。

(iii)$\Rightarrow$(iv): 性質(iii)が成り立つと仮定します。この場合、$L_{(\Omega )}$ は代数 Ω[G] 上の階数 1 の自由加群です。後者は $K[G]_{(\Omega )}$ で正規に識別できます。次に、定理を適用する 3 の VIII、p. 37 となります。

含意 (iv)$\Rightarrow$(v) は明らかです。

含意 (v)$\Rightarrow$(vi) を証明しましょう。 代数 L が減少します。 補題 8、c) により、群 G は L の最大理想の集合 $\mathscr{S}$ に推移的に作用します。 $\mathfrak{m}$を$\mathscr{S}$の元とします。 $\bigcap_{\mathfrak{n}\in\mathscr{S}}\mathfrak{n}=\{0\}$ 以降、補題 9 までに、代数 L は代数 Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ と同型です。 $L/\mathfrak{m}$ における $G_{\mathfrak{m}}$ の不変式の代数したがって、K による補題 7 による一致する、c)。したがって、$G_{\mathfrak{m}}$ から Gal((L$/\mathfrak{m}$)$/K$) への準同型 $\lambda_{\mathfrak{m}}$ は全射法です。 補題 7 までに、さらに

カード(G) $= [L : K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]$。従って、Card(G$_{\mathfrak{m}}$) $= [L/\mathfrak{m}: K]$、および準同型 $\lambda_{\mathfrak{m}}$ は単射法です。

含意 (vi)$\Rightarrow$(i) を証明することはまだ残っています。 $\mathfrak{m}$ をL の最大の理想とする。 補題 9 により、代数 L は $(K$、G)-代数として代数 Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$ と同型です。 $G_{\mathfrak{m}}$ は $L/\mathfrak{m}$ で忠実に動作し、K を不変式の部分体として認めるので、$G_{\mathfrak{m}}$ から Gal((L$/\mathfrak{m}$)$/K$) まで、群準同型 $\lambda_{\mathfrak{m}}$ 定義する同型となります。

#### 注意 2 {#alg-viii-s16-n7-rem-2 .statement tag=00J2}

定理 2 では、Ω が可分に閉じているという仮定によって Ω が代数的に閉じているという置き換える仮定ができます。確かに、L がエタールであれば、L から Ω までのすべての K-代数準同型の像は K の分離拡大です。

#### 注意 3 {#alg-viii-s16-n7-rem-3 .statement tag=00J3}

通常の基底定理 (V, §10, No. 9、p. 73、定理 6) は、定理 2 の含意 (i)$\Rightarrow$(iv) の特定のケースです。

#### 定義 1 {#alg-viii-s16-def-1 .statement tag=00J4}

Gを有限群とし、Lを$(K,G)$-代数の構造を備えたK上の有限次数の非零可換代数とする。ここで、Gの作用はGから群への単射準同型によって与えられる。 8月$_K(L)$。 定理 2 と同等の性質 (i) から (vi) を持っている場合、L は群 G を持つガロア代数であると言います。

#### 注意 4 {#alg-viii-s16-n7-rem-4 .statement tag=00J5}

L が G の作用 $\lambda$ を備えた K の拡大であるとします。そのとき、L が K のガロア拡大であり、$\lambda$ が G から同型である場合に限り、L は K よりガロア代数になります。 L中ガロア群がKを上回りました。

#### 注意 5 {#alg-viii-s16-n7-rem-5 .statement tag=00J6}

群 G がアーベルであるとします。 G が集合 X に対して忠実かつ推移的に作用する場合、X の任意の点の固定群は恒等式に還元されます (X の点の固定群はすべて等しく、それらの共通部分は G の単位元に還元されるため)。従って、定理 2 の性質 (i) から (vi) も次と等価です。

(vii) 代数 L はエタールであり、G は$\mathscr{H}$ に対して忠実かつ推移的に作用します。

#### 注意 6 {#alg-viii-s16-n7-rem-6 .statement tag=00J7}

V, §10, No. 1、p. 75、補題 5 まで。 V, §10, No. 1、p. 76、命題 12; VIII、p. 137、命題 3、ガロア代数は可換であり、半単純。

#### 例 1 {#alg-viii-s16-n7-exa-1 .statement tag=00J8}

$n$ を、K の特性指数の素数である厳密な正の整数とします。K の単位元の $n$ 番目の根の群 $\mu_n$ が位数 $n$ を持つとします。次に、$n$ の因子 $d$ ごとに、単位元の $d$ 番目の根の群 $\mu_d$ は位数 $d$ になります。 $a$ を K の非零元とし、L を代数 $K[X]/(X^n-a)$ とし、$x$ を L の X の類とします。 数列 $(1, x, . . . , x^{n-1})$ は、体 K を超えるベクトル空間 L の基底で、$x^n=a$ があります。さらに、多項式 $X^n-a$ はその導関数 $nX^{n-1}$ に対して素数であるため、代数 L はエタール (V, §7, No. 2, p. 37, 命題 3) です。 $\mu_n$ の $\zeta$ ごとに、環 K[X] 定義するの自己同型 $P(X)\mapsto P(\zeta X)$、移行から商、自己準同型 $\lambda (\zeta )$ までL は $(\zeta X)^n-a= X^n-a$ があるためです。 自己同型です。我々は持っています

$$
\lambda (\zeta )x^i=\zeta^ix^i \tag{19}
$$

$0\leqslant i < n$の場合。 写像 $\lambda :\zeta \mapsto \lambda (\zeta )$ は $\mu_n$ から Aut$_K$(L) までの単射準同型であり、L の群 $\lambda (\mu_n)$ の不変量の環は $K\cdot 1$ に等しい。 $\mu_n$の基数は$n= [L : K]$に等しいので、$\lambda$の作用が付与された代数Lはガロア代数になります(VIII, p. 308, 定理 2, (v))。

$r$ を、$a^r$ 属するから $K^{*n}$ となるような最小の厳密な正の整数とします。それは割る $n$ であり、$a=b^{n/r}$ となる $K^*$ の元 $b$ が存在します。すると (V, §11, No. 8, p. 91, 注意) 多項式 $X^r-b$ は既約で、$X^n-a=\prod_{\zeta\in\mu_{n/r}}(X^r-\zeta b)$ が得られます。 E を体 $K[Y]/(Y^r-b)$ とし、$y$ を E の Y の類とします。$\mu_{n/r}$ から Gal(E$/K$) まで同型 $\theta$ が存在し、関係 $\theta (\xi )(y) =\xi y$ によって特徴付けられます。 (V, §11, No. 8、p. 91、例 3)。次に、ガロア代数 L が $(K, \mu_n$)-代数 Coind$^{\mu_n}_{\mu_{n/r}}(E)$ と同型であることを検証します。

#### 例 2 {#alg-viii-s16-n7-exa-2 .statement tag=00J9}

ここで、体 K が特性 $p\not= 0$ を持っているとします。 $c$ を K の元とします。多項式 $f= X^p-X-c$ はその導関数 $f'=-1$ に対して素数であるため、代数 $L = K[X]/(f)$ はエタール (V, §7, No. 2, p. 37, 命題 3) です。 LのXの像を$x$で表します。 関係 $x^p=x+c$ があります。 数列 $(1, x, . . . , x^{p-1})$ は、K 上のベクトル空間として見られる L の基底です。

P を K の素数部分体の加法群とします。これは、位数 $p$ の巡回群であり、K の単位元 1 によって生成されます。P のすべての $j$ に対して、$j^p=j$ (V, §1, No. 3, p. 4, 公式 (4)) が得られます。 $f(X +j) =f(X)$。したがって、関係 $\gamma (j)(x) =x+j$ によって特徴付けられる代数 L の自己同型 $\gamma (j)$ が存在します。さらに、結果として得られる写像 $\gamma$ は、P から Aut$_K(L)$ までの単射準同型です。

Ω を K の代数閉拡大とし、$\xi$ を Ω の多項式 $f$ の根とします。 $\xi^p=\xi +c$ があるため、

$$
X^p-X-c= (X^p-\xi^p)-(X-\xi ) = (X-\xi )^p-(X-\xi ) =\prod_{j\in P}(X-\xi -j)
$$

V, §12, No. 1、p. 94、公式作 (1)。 P のすべての $j$ に対して、$x$ を $\xi +j$ に送信する一意な代数準同型 $\chi_j: L\rightarrow \Omega$ が存在します。さらに、L から Ω までのすべての準同型は $\chi_j$ の 1 つであり、関係 $\chi_j=\chi_0\circ \gamma (j)$ があります。 $\gamma$ を備えた代数 L は、定理 2 の VIII、p. 308 の性質 (ii) を持っているため、K よりもガロア代数です。

L の構造を説明するには、2 つのケースを区別する必要があります。

a) $\xi \notin K$ があります。このとき、多項式 $f(X)$ は K[X] (V, §11, No. 9, p. 93, 例 3) で既約です。この場合、Lは次数$p$のKの巡回拡大であり、$\gamma$はPからGal(L$/K$)までの同型です。

b) $\xi \in K$ があります。すると、写像 $\psi :y\mapsto (\chi_j(y))_{j\in P}$ は、代数 L から積代数 $K^P$ までの同型です。さらに、$\psi \circ \gamma (k)\circ \psi^{-1}$ は、$k\in P$ ごとに $K^P$ の自己同型 $(x_j)_{j\in P}\mapsto (x_{j+k})_{j\in P}$ です。

### 8. ガロア代数の作用

#### 命題 9 {#alg-viii-s16-prop-9 .statement tag=00JA}

Gを有限群、HをGの部分群、Eを群Hと体K以上のガロア代数とします。すると、HからGへの共帰によってEから導出される$(K,G)$-代数Coind$^G_H(E)$はガロア代数以上となります。 体 K と群 G.

E は K よりガロア代数なので、VIII の定理 2、p. 308 の性質 (v) によって減算され、Card(H) = [E : K] が得られ、K は E における H の不変量の環になります。ただし、補題によってVIII、p. 305、代数 F = Coind$^G_H(E)$ の 7 が減らされ、

[F : K] = (G : H)[E : K] = (G : H) カード(H) = カード(G)、

そして、K は F における G の不変量の環です。したがって、定理 2、(v) で与えられる基準により、F はガロア代数です。

#### 命題 10 {#alg-viii-s16-prop-10 .statement tag=00JB}

G を有限群とします。 L を群 G を持つ体 K 上のガロア代数とし、$K'$ を K の拡大とします。すると、$(K',G)$-代数 $L_{(K')}$ は $K'$ 上のガロア代数となります。

観察するとによる定理 2 の性質 (v) を使用すると、K-代数 L がエタールである場合、$K'$-代数 $L_{(K')}$ も (V, §6, No. 5, p. 32, 系 2) になります。 等式 $[L_{(K')}: K'] = [L : K]$ があり、$L_{(K')}$ の G の不変量の環は $(L^G)_{(K')}$ で、$L^G$ は L の G の不変量の環です。

#### 命題 11 {#alg-viii-s16-prop-11 .statement tag=00JC}

$G_1$ と $G_2$ を群とします。 $L_1$ と $L_2$ を、それぞれ作用 $\lambda_1: G_1\rightarrow$ Aut$_K(L_1)$ と $\lambda_2: G_2\rightarrow$ Aut$_K(L_2)$ を伴う K 上のガロア代数とします。 集合 $L = L_1\otimes_KL_2,G = G_1\times G_2$、$(g_1, g_2)\in G$ の場合は $\lambda (g_1, g_2) =\lambda_1(g_1)\otimes \lambda_2(g_2)$。すると、作用 $\lambda$ が備わったK-代数 L は、K よりガロア代数になります。

以下を考慮して、前にと推論します。 $L_1$ と $L_2$ がエタールである場合、代数 $L = L_1\otimes_KL_2$ (V, §6, No. 5, p. 32, 系 1) も同様であり、等式が成り立ちます。

$[L : K] = [L_1: K][L_2: K]$ およびカード(G) = カード(G$_1$) カード(G$_2$)。

さらに、$L^{G_i}_i$ が $L_i$ の $G_i$ の不変量の環を表す場合、以下の補題 11 から、$L^{G_1}_1\otimes_KL^{G_2}_2$ は $L_1\otimes_KL_2$ の $G_1\times G_2$ の不変量の環であることがわかります。

#### 補題 11 {#alg-viii-s16-lem-11 .statement tag=00JD}

$G_1$ と $G_2$ を群とし、$W_1$ と $W_2$ を K-ベクトル空間とします。私たちはそれぞれ$W_1($を寄付します。 $W_2)$ と $G_1($ の作用 $G_2)$ は群準同型 $\rho_1: G_1\rightarrow$ Aut$_K(W_1) ($ によって与えられました。 $\rho_2: G_2\rightarrow$ 8月$_K(W_2))$。 群準同型を検討します

$\rho_1\otimes \rho_2: G_1\times G_2\longrightarrow$ 秋$_K(W_1\otimes_KW_2)$

$g_1\in G_1,g_2\in G_2,w_1\in W_1$ および $w_2\in W_2$ の関係 $(\rho_1\otimes \rho_2)(g_1, g_2)(w_1\otimes w_2) =\rho_1(g_1)(w_1)\otimes \rho_2(g_2)(w_2)$ によって定義されます。 次に、$W^{G_1}_1\otimes_KW^{G_2}_2$から$W_1\otimes_KW_2$までの線形写像は、標準単射の誘導する同型、$W_1^{G_1}\otimes_KW^{G_2}_2$から$(W_1\otimes_KW_2)^{G_1\times G_2}$のK-ベクトル空間のテンソル積によって与えられます。

This follows from Lemma 1 of VIII, p. 213 applied to the K[G]-modules $M_1= M_2= K$ endowed with the trivial action of $G, N_1= W_1$, and $N_2= W_2$.

#### 注意 {#alg-viii-s16-n8-rem-1 .statement tag=00JE}

L を有限次数の体 K のガロア拡大とし、G をそのガロア群とします。 G 上の恒等写像を $\lambda$ で表します。 すると、$\lambda$ を備えたL は、群 G で K を超えてガロア代数になります。 $K'$ を K の拡大とします。 命題 10 までに、代数 $L_{(K')}$ は $K'$ を超えるガロアですが、一般的には $K'$ の拡大ではありません。 同様に、命題 11 により、ガロア拡大 E のテンソル積と有限次数の K の F はガロア代数と見なすことができます。一般に、それは K のガロア拡大ではありません。 ただし、E と F が K の拡大の線形互いに素部分拡張である場合 (V, §2, No. 5、p. 13 および V, §10, No. 1、p. 57、命題 1) は 1 です。

### 9. 外積

K を体、G を群とし、その単位元を $e$ で表します。 L を可換K-代数とし、$\lambda$ を G から K-代数 L の自己同型群までの準同型とします。 G の任意の $g$ について、$\tau (g)$ を、$\lambda (g)$ によって誘発された乗法群の自己同型 L の $L^*$ とします。

$\mathscr{E}= (\Gamma , \iota , \pi )$ を群 G の $L^*$ による $\tau$ 拡張とする。 集合 $L\times \Gamma$ の定義する右作用の群 $L^*$

$$
(\beta , \gamma ).\alpha = (\beta \alpha , \iota (\alpha )^{-1}\gamma ) \tag{20}
$$

$\alpha \in L^*,\beta \in L$ と $\gamma \in \Gamma$ の場合。 We denote by E the set of orbits of $L^*$ in $L\times \Gamma$ and by $[\beta ;\gamma ]$ the orbit of the pair $(\beta , \gamma )$. したがって、構成までに関係になります

$$
[\beta \alpha ;\gamma ] = [\beta ;\iota (\alpha )\gamma ] \tag{21}
$$

$\alpha \in L^*,\beta \in L$ と $\gamma \in \Gamma$ の場合。

L の $\beta$ と Γ の $\gamma$ を考えると、L の自己同型 $\lambda \circ \pi (\gamma )$ の下の $\beta$ の $^{\gamma}\beta$ 変換によって表されます。 関係があります

(22) $^{\gamma}(^{\gamma'}\beta ) =^{\gamma \gamma'}\beta  ,^{\gamma}(\beta +\beta ') =^{\gamma}\beta +^{\gamma}\beta '$ と $^{\gamma}(\beta \beta ') =^{\gamma}\beta^{\gamma}\beta '$

Γの$\gamma , \gamma '$とLの$\beta , \beta '$。 関係を特徴とする E には合成の法則が存在します

$$
[\beta ;\gamma ][\beta ';\gamma '] = [\beta^{\gamma}\beta ';\gamma \gamma '] \tag{23}
$$

確かに、$L^*$ のすべての $\alpha ,\alpha '$ について、それぞれ置き換える、$\beta ,\gamma ,\beta '$、$\gamma '$ と $\beta \alpha ,\iota (\alpha )^{-1}\gamma ,\beta '\alpha '$、および $\iota (\alpha ')^{-1}\gamma '$ をとった場合、右辺は変更にならないことを検証するだけで十分です。この直後に、VIII、p. 285 の適用から $\mathscr{E}$ 公式が続きます。これは、$\gamma \in \Gamma$ と $\alpha \in L^*$ に対して $\gamma \iota (\alpha ) =\iota (^{\gamma}\alpha )\gamma$ と書くこともできます。 (22) の公式により、この法則を備えた集合 E は単位元 $[1;e]$ とのモノイドになります。

$\pi \circ \iota$ は値 $e$ で定数であるため、E から G までの写像 $\widetilde{\pi}$ が存在し、次のようになります。

$$
\widetilde{\pi}([\beta ;\gamma ]) =\pi (\gamma ) \tag{24}
$$

$\beta \in L$ と $\gamma \in \Gamma$ の場合。

$g$をGの元とし、$E_g=\widetilde{\pi}^{-1}(g)$とします。 $\gamma_0$ が $\pi^{-1}(g)$ の固定元である場合、写像 $\beta \mapsto [\beta ;\gamma_0]$ は L から $E_g$ までの全単射となり、そのおかげで $E_g$ K-ベクトル空間構造に転送されます。 L。 $\pi^{-1}(g)$ は形 $\iota (\alpha )\gamma_0$ の元で構成されているため、$\alpha$ は $L^*$ まで続き、次のようになります。

$$
[\beta ;\iota (\alpha )\gamma_0] = [\beta \alpha ;\gamma_0]
$$

$E_g$ のベクトル空間構造は、$\gamma_0$ の選択に依存しません。

$g$ と $g'$ を G の元とします。 公式 (22) と (23)、E 誘導するの合成の法則による、制限による、$E_g\times E_{g'}$ から $E_{gg'}$ までの K 双線形写像。その結果、ベクトル空間 $P =\bigoplus_{g\in G}E_g$ には、結合的で単位的な代数の構造が与えられ、その乗法誘導するは、すべての $g$ について $E_g\times E_{g'}$ から $E_{gg'}$ までの以前の双線形写像となり、 G の $g'$。代数 P は、L と $\mathscr{E}$ の外積と呼ばれ、$\mathbf{A}[\mathscr{E}; L]$ で表されます。その単位元は $E_e$ の元 $[1;e]$ です。

集合

$$
u(\beta ) = [\beta ;e] \tag{25}
$$

Lの$\beta$用。すると、$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$はK-代数の単射準同型になります。 (23) により、$\gamma \in \Gamma$ ごとに、元 $[1;\gamma ]$ は $\mathbf{A}[\mathscr{E},L]$ で可逆であり、$\gamma$ を $[1;\gamma ]$ に送る写像 $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E},L]^*$ は単射法群準同型になります。 準同型 $u$ と $v$ は正規と呼ばれます。 関係があります

$$
u(\alpha ) =v(\iota (\alpha )) \tag{26}
$$

$$
u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1} \tag{27}
$$

$$
[\beta ;\gamma ] =u(\beta )v(\gamma ) \tag{28}
$$

$\alpha \in L^*,\beta \in L$と$\gamma \in \Gamma$の場合。

逆に、代数 $\mathbf{A}[\mathscr{E}; L]$ の次の普遍性があります。

#### 命題 12 {#alg-viii-s16-prop-12 .statement tag=00JF}

B を K-代数、$u': L\rightarrow B$ K-代数準同型、$v': \Gamma \rightarrow B^*$ 群準同型とします。満足していると仮定します関係

$$
u'(\alpha ) =v'(\iota (\alpha )) \tag{29}
$$

$$
u'(^{\gamma}\beta ) =v'(\gamma )u'(\beta )v'(\gamma )^{-1} \tag{30}
$$

$\alpha \in L^*,\beta \in L$、および$\gamma \in \Gamma$の場合。次に、$\mathbf{A}[\mathscr{E}; L]$からBまで一意な代数準同型$f$が存在し、$u'=f\circ u$と$v'=f\circ v$が存在します。

To prove the uniqueness of $f$, observe that the vector space $\mathbf{A}[\mathscr{E}; L]$ over the field K is generated by the set of elements of the form $[\beta ;\gamma ] =u(\beta )v(\gamma )$. 準同型 $f':\mathbf{A}[\mathscr{E}; L]\rightarrow B$ が $f'\circ u=u'$ と $f'\circ v=v'$ を満たす場合、$[\beta ;\gamma ]$ を $u'(\beta )v'(\gamma )$ に送信し、従って $f$ とともに一致するを送信します。

公式 (29) までに、

$$
u'(\beta \alpha )v'(\iota (\alpha )^{-1}\gamma ) =u'(\beta )v'(\gamma ) \tag{31}
$$

$L^*,\beta$のLの$\alpha$、およびΓの$\gamma$。 E の定義により、結果として $f_0([\beta ;\gamma ]) =u'(\beta )v'(\gamma )$ となる写像 $f_0: E\rightarrow B$ が存在します。 公式 (23) と (30) により、E の $x$ と $x'$ に対して $f_0(xx') =f_0(x)f_0(x')$ が得られます。 $f_0$ から $E_g$ の制限は、G の元 $g$ ごとに K 線形です。従って、$\mathbf{A}[\mathscr{E}; L]$からBまで一意なK-線型写像$f$が存在し、Eに$f_0$を持つ一致するが存在します。写像$f$は$u'=f\circ u$を満たす代数射であり、 $v'=f\circ v$。

#### 注意 {#alg-viii-s16-n9-rem-1 .statement tag=00JG}

$\sigma : G\rightarrow \Gamma$ を写像 $\pi$ の切断とします。 G のすべての $g$ に対して集合 $\varepsilon_g=v(\sigma (g))$ を表し、$\sigma$ (VIII、p. 296) に関連付けられた 2 共環を $c_{\sigma}$ で示します。特に、私たちは、

$$
\varepsilon_g\varepsilon_{g'}=u(c_{\sigma}(g, g'))\varepsilon_{gg'} \tag{32}
$$

すべての$g, g'\in G$に。 さらに、準同型 $u$ を介して、$\mathbf{A}[\mathscr{E}; L]$ の部分代数を同一視する L とします。 次に、$\mathbf{A}[\mathscr{E}; L]$ のすべての元は、$\sum_{g\in G}a_g\varepsilon_g$ として一意に書くことができます。ここで、$(a_g)$ は、有限台を含む L の元のファミリーです。 $\mathbf{A}[\mathscr{E}; L]$の乗法は公式で表現できます

$$
(\sum_ga_g\varepsilon_g)(\sum_gb_g\varepsilon_g)=\sum_gd_g\varepsilon_g \tag{33}
$$

と

$$
d_g=\sum_{hh'=g}a_h(\lambda (h)\cdot b_{h'})c_{\sigma}(h, h') \tag{34}
$$

拡大 $\mathscr{E}$ が半自明である場合、$\pi$ の選ぶ切断 $\sigma$、つまり G から Γ までの群射ができます。従って、共循環 $c_{\sigma}$ は値 1 で定数となり、公式 (34) は次のように単純化されます。

$$
d_g=\sum_{hh'=g}a_h\lambda (h)\cdot b_{h'} \tag{35}
$$

$K'$ を体 K の拡大とします。 $L'$ で $K'$-代数 $L_{(K')}$ を表し、G の任意の $g$ について、 $\lambda (g)$ によって誘導される $\lambda '(g)$ 自己同型 $\lambda (g)_{(K')}$ で表します。 $L_{(K')}$に。さらに、$\lambda '(g)$によって引き起こされた$L^{'*}$の$\tau '(g)$自己同型で表すことにします。最後に、$h$ を $L^*$ から $L^{'*}$ までの準同型として、$x$ を $x\otimes 1$ に送信します。 $\mathscr{E}'= (\Gamma ', \iota ', \pi ')$ を $\mathscr{E}$ の拡大から $h$ (VIII, p. 289) までの直像とします。 $\mathbf{A}[\mathscr{E}',L']$ を外積 $\mathscr{E}'$ と $L'$ の代数 $K'$ とし、$u': L'\rightarrow \mathbf{A}[\mathscr{E}',L']$ と $v': \Gamma '\rightarrow \mathbf{A}[\mathscr{E}',L']^*$ を標準準同型とします。

#### 命題 13 {#alg-viii-s16-prop-13 .statement tag=00JH}

関係を満たす$\mathbf{A}[\mathscr{E}; L]_{(K')}$ から $\mathbf{A}[\mathscr{E}'; L']$ までの$K'$-代数$\varphi$ のうち、関係を満たす固有の同型が存在します。

$$
u'(h(\beta )) =\varphi (1\otimes u(\beta )) \tag{36}
$$

$\beta \in L$ と

$$
v'(h(\gamma )) =\varphi (1\otimes v(\gamma )) \tag{37}
$$

$\gamma \in \Gamma$の場合。

構成の直後に証明が続きます。

同型 $\varphi$ は正規と呼ばれます。

### 10. ブラウアー群へのお申込み

この小節では、Kは体、Lは作用$\lambda : G\rightarrow$Aut$_K(L)$でKを超えてガロア代数です。 K 上の L の次数を $n$ で表します。 $n=$ カード(G)を所持しております。

#### 定理 3 {#alg-viii-s16-thm-3 .statement tag=00JI}

$\mathscr{E}= (\Gamma , \iota , \pi )$ を $L^*$ による G の $\tau$ 拡張とする。 代数 $\mathbf{A}[\mathscr{E}; L]$ は中心単純であり、K 上の次数 $n^2$ です。さらに、L から $\mathbf{A}[\mathscr{E}; L]$ までの標準準同型 $u$ は、L から最大値までの同型です。 $\mathbf{A}[\mathscr{E}; L]$中可換部分代数。

#### 補題 12 {#alg-viii-s16-lem-12 .statement tag=00JJ}

a) G の下で不変である $\{0\}$ と L 以外に、L のイデアルは存在しません。

b) $g$ を単位元とは異なる G の元とし、$\mathfrak{a}_g$ を形 $x-\lambda (g)x$ の元によって生成される L の理想とし、ここで $x$ は L を通過します。 $\mathfrak{a}_g= L$があります。

$\mathscr{S}$ を最大理想 L の集合とします。 $\mathscr{S}$、集合 $\mathfrak{a}(S) =\bigcap_{\mathfrak{m}\in S}\mathfrak{m}$ のいずれかの部分集合 S の場合。 環 L は可換であり、半単純 (VIII, p. 310, 注意 6) であるため、写像 $W\mapsto \mathfrak{a}(W)$ は、部分集合の集合から全単射になります。 L（VIII、p. 142、命題9）の理想の$\mathscr{S}$から集合。イデアル $\mathfrak{a}(S)$ は、S が存在する場合に限り、G の下で不変です。 G は $\mathscr{S}$ (VIII, p. 308, 定理 2, vi)) に対して推移的に作用するため、G の下で不変となる $\mathscr{S}$ のうち部分集合は $\emptyset$ と $\mathscr{S}$ だけです。 $\mathfrak{a}(\emptyset ) = L$ と $\mathfrak{a}(\mathscr{S}) =\{0\}$ 以来、主張 a) が証明されました。

b) を矛盾によって証明しましょう。 $\mathfrak{a}_g\not= L$ があるとします。 $\mathfrak{m}$ を L 含む $\mathfrak{a}_g$ の最大理想とする。次に、L のすべての $x$ に対して $\lambda (g)x\equiv x$ mod $\mathfrak{m}$ が得られます。特に、$\mathfrak{m}$ は $g$ の下で不変であり、$\lambda (g)$ は体 $L/\mathfrak{m}$ 上の同一性によって誘導されます。 性質 (vi) により、VIII、p. 308、元 $G_{\mathfrak{m}}$ の $g$ の定理 2 は自明であり、b) の矛盾する仮定です。

ここで、定理 3 を証明しましょう。 ベクトル空間 $\mathbf{A}[\mathscr{E}; L]$ は、VIII、p. 316 と仮定された等式カード(G) $= [L : K] =n$ によって、K 上に有限次元カード(G)[L$: K] =n^2$] を持っています。

$\mathfrak{a}$ を代数 $\mathbf{A}[\mathscr{E}; L]$ の両側理想である非零とします。 VIII、p. 316の記法を使用します。 $\mathbf{A}[\mathscr{E}; L]$ のすべての元 $a$ は、$g\in G$ ごとに $a_g\in L$ を含む $a=\sum_{g\in G}a_g\varepsilon_g$ として一意に書くことができます。 $a_g\not= 0$ のような G の元 $g$ を $\Phi (a)$ 集合で表します。 VIII、p. 316 の公式 (32) までに、関係になります

$$
\varepsilon_g\varepsilon_{g'}=c_{\sigma}(g, g')\varepsilon_{gg'} \tag{38}
$$

すべての$g, g'\in G$にとって、そしてその結果として

$$
\Phi (a\varepsilon_g) = \Phi (a).g \tag{39}
$$

$g\in G$ と $a\in \mathbf{A}[\mathscr{E}; L]$ ごとに。

$a$ を $\mathfrak{a}$ の非零元とし、$\Phi (a)$ が包含の最小値であるとします。 公式 (39)、必要に応じて置き換えること $a$ と形の元 $a\varepsilon_{g^{-1}}$ と $g\in \Phi (a)$ を組み合わせると、$e\in \Phi (a)$ があると仮定できます。 $s$ を $e$ から区別する $\Phi (a)$ の元とします。 補題 12、b) までに、$a_s(x-\lambda (s)\cdot x)\not= 0$ となる L の元 $x$ が存在します。しかし、私たちには関係があります

$$
xa-ax=\sum_ga_g(x-\lambda (g)\cdot x)\varepsilon_g \tag{40}
$$

ここで、和は、$e$ とは異なり、$\Phi (a)$ の元 $g$ を引き継ぎます。 $\Phi (a)$ が最小であるため、次に $xa-ax= 0$ が得られますが、これは $x$ で矛盾する仮定になります。従って、G の $\Phi (a)$ 含むは単位元 $e$ のみであることが矛盾によって証明されたので、$a\in L$ になります。

従って、$L\cap \mathfrak{a}$ は、$\{0\}$ に還元されない L の理想です。さらに、L のすべての $x$ に対して、$\varepsilon_gx\varepsilon^{-1}_g=\lambda (g)\cdot x$ が得られるため、$L\cap \mathfrak{a}$ は G の下で不変です。従って、補題 12 までに、$L\cap \mathfrak{a}= L$、つまり $L\subset \mathfrak{a}$ が得られます。 $\mathbf{A}[\mathscr{E}; L]$ の L 含む単位元なので、$\mathfrak{a}=\mathbf{A}[\mathscr{E}; L]$ になります。

代数 $\mathbf{A}[\mathscr{E}; L]$ は K に対して非零有限次元を持ち、その両側の理想は $\{0\}$ と $\mathbf{A}[\mathscr{E}; L]$ だけなので、単純です。

$\mathbf{A}[\mathscr{E}; L]$ のすべての元 $a$ が L 属するから L と可換であることを証明しましょう。 Lに係数$a_g$を入れて、$a$を$\sum_{g\in G}a_g\varepsilon_g$と書きます。 L の各 $x$ に対して、$xa-ax= 0$ があり、関係 (40) は、

$$
a_g(x-\lambda (g)\cdot x) = 0 \tag{41}
$$

$g\in G$ と $x\in L$ ごとに。従って、補題 12 までに、$g\not=e$ に対して $a_g= 0$ が得られます。従って、$a\in L$。

最後に、$\mathbf{A}[\mathscr{E}; L]$ の決定する中心を見てみましょう。 $z$ 属するから中心の場合、L と交換するため、属するから L になります。しかし、その後、

$$
0 =\varepsilon_gz-z\varepsilon_g= (\lambda (g)\cdot z-z)\varepsilon_g
$$

G の $g$ ごとに。 従って、$z$ は L の自己同型群 $\lambda (G)$ の下で不変です。 従って、仮定までに$z\in K$が得られます。

#### 定理 4 {#alg-viii-s16-thm-4 .statement tag=00JK}

A を K 上の有限次数の中心単純代数とし、L を A の最大値可換部分代数とする。すると、A が $\mathbf{A}[\mathscr{E}; L]$ と同型となるように、G の $L^*$ による $\tau$ 拡張 $\mathscr{E}$ が存在する。

一般性を失うことなく、L は A の最大可換部分代数であると仮定できます。 Γ を A の可逆元 $\gamma$ の乗法群からなるとし、次の条件を満たす G に $g$ が存在します。

$$
\gamma x\gamma^{-1}=\lambda (g).x \tag{42}
$$

L の元 $x$ ごとに。 $\gamma \in \Gamma$ が与えられた場合、元 $g$ 満たすこの関係は一意です。それを$\pi (\gamma )$で表します。 $\pi$がΓからGまで準同型であり、その核が$L^*$に等しいのは明らかです。 $\pi$ の全射性は、スコレム・ネーター 定理 (VIII、p. 263、系) に続きます。

$L^*$の標準単射を$\iota$でΓに表すと、構成から、$\mathscr{E}= (\Gamma , \iota , \pi )$はGの$L^*$による$\tau$拡張であることがわかります。させて

$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ と $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E}; L]$

標準準同型になります。 $\mathbf{A}[\mathscr{E}; L]$ (VIII, p. 315, 命題 12) の普遍性により、$x\in L$ に対して $f\circ u(x) =x$ と $f\circ v(\gamma ) =\gamma$ が成り立つ一意な代数準同型 $f:\mathbf{A}[\mathscr{E}; L]\rightarrow A$ が存在します。 $\gamma \in \Gamma$。 代数 $\mathbf{A}[\mathscr{E}; L]$ は単純なので、準同型 $f$ は単射法です。さて、代数 $\mathbf{A}[\mathscr{E}; L]$ は K に対して次数 $n^2$ を持ち、A も同様です。なぜなら、L は A の最大可換半単純部分代数であり、$n= [L : K]$ (VIII, p. 262, 命題) があるからです。 3、(ii))。したがって、$f$ は全単射です。

#### 定義 2 {#alg-viii-s16-def-2 .statement tag=00JL}

$\mathscr{S}$を最大理想Lの集合とします。私たち定義する

Br(L$/K$) $=\bigcap_{\mathfrak{m}\in\mathscr{S}}$ Ker($r_{(L/\mathfrak{m})/K}$)、ここで $r_{(L/\mathfrak{m})/K}:$ Br(K) $\rightarrow$ Br(L$/\mathfrak{m}$) はスカラー 準同型の拡大 (VIII、p. 281)。

#### 定理 5 {#alg-viii-s16-thm-5 .statement tag=00JM}

群同型が存在します

Ψ : 元$_{\tau}(G,L^*)\longrightarrow$ Br(L$/K$)

これは、G の $\tau$ 拡張 $\mathscr{E}$ の $L^*$ の類を、代数 $\mathbf{A}[\mathscr{E}; L]$ の Br(L$/K$) の類に送信します。

定義する Ψ を検証し、それが全単射であることを検証するには、次の点を確立する必要があります。

a) $\mathscr{E}$ と $\mathscr{E}'$ が $L^*$ による G の同型 $\tau$ 拡張である場合、代数 $\mathbf{A}[\mathscr{E}; L]$ と $\mathbf{A}[\mathscr{E}'; L]$ は同型です。

b) 逆に、代数 $\mathbf{A}[\mathscr{E}; L]$ と $\mathbf{A}[\mathscr{E}'; L]$ が同型である場合、$L^*$ による G の $\tau$ 拡張 $\mathscr{E}$ と $\mathscr{E}'$ は同型です。

c) Br(L$/K$) のすべての類には、最大可換部分代数として代数 E 含む L があります。

d) E が、極大値可換部分代数として K 含む L 上の有限次数の中心単純代数である場合、E が $\mathbf{A}[\mathscr{E}; L]$ と同型となるように、$L^*$ による G の $\tau$ 拡張$\mathscr{E}$ が存在します。

主張 a) 外積の構成から続きます。 b) VIII、p. 263、系から続きます。 主張 c) は、VIII、p. 281 の命題 5 から続き、d) は単に上記の定理 4 です。

Ψ が群準同型であることを確認する必要があります。このためには、$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$ と $\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$ が $\tau$ 拡張である場合、代数 $\mathbf{A}[\mathscr{E}_1\mathscr{E}_2; L]$ は代数 $\mathbf{A}[\mathscr{E}_1; L]\otimes \mathbf{A}[\mathscr{E}_2; L]$ と同等であることを証明すれば十分です。 積拡大 $\mathscr{E}_1\mathscr{E}_2$ を $\mathscr{E}= (\Gamma , \iota , \pi )$ で表します。 群 Γ は、$L^*$ から$\mu$ を$(\iota_1(\mu), \iota_2(\mu)^{-1})$ に送信するファイバー 積 $\Gamma_1\times_G\Gamma_2$ の準同型 $\rho$ の余核と同型です。 $i\in  \{1,2\}$の場合は、$A_i=\mathbf{A}[\mathscr{E}_i; L]$と記入してください。 $u_i: L\rightarrow A_i$と$v_i: \Gamma_i\rightarrow A^*_i$を標準準同型とします。私たちは同一視する L とその像を準同型 $u_i$ で計算し、L を$A_i$ の最大可換部分代数とします。 $A_i$ の左乗法によって定義される L ベクトル空間を $V_i$ で表します。 環 $L\otimes_KA^o_i$ は $V_i$ に作用します。単純で、Lの上に次元$n^2$があるので、$L\otimes_KA^o_i$からEnd$_L(V_i)$まで同型が得られます。したがって、$(L\otimes_KA^o_1)\otimes_L(L\otimes_KA^o_2)$ と同一視できるを結合した環 $L\otimes_KA^o_1\otimes_KA^o_2$ は End$_L(V_1\otimes_LV_2)$ と同型です。 集合 C = 終了$_{A^o_1\otimes_KA^o_2}(V_1\otimes_LV_2)$。 VIII、p. 282、環 C の補題 3 は $A_1\otimes_KA_2$ に似ており、$L\otimes 1\otimes 1$ は C の最大可換部分代数です。すべての対 $(\gamma_1, \gamma_2)\in \Gamma_1\times \Gamma_2$ 満たす $\pi_1(\gamma_1) =\pi_2(\gamma_2)$ について、次のような一意の $\lambda (\pi_1(\gamma_1$)) 半線形 (II, §1, No. 13, p. 223) 自己準同型を $w(\gamma_1, \gamma_2)$ で表します。

$$
w(\gamma_1, \gamma_2)(x_1\otimes x_2) =v_1(\gamma_1)x_1\otimes v_2(\gamma_2)x_2
$$

$x_1\in V_1$ と $x_2\in V_2$ 用。 $w(\gamma_1, \gamma_2)\in C^*$ があり、$w$ はファイバー 積 $\Gamma_1\times_G\Gamma_2$ から $C^*$ の群準同型です。この準同型は、Γから$C^*$までの$\rho$の像と誘導する準同型$v$では自明です。 $u:\ell \mapsto \ell \otimes 1\otimes 1$ によって与えられる $u: L\rightarrow C$ 射で表します。 関係を確認できます

$u(\alpha ) =v(\iota (\alpha ))$ と $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$

$\alpha \in L^*,\beta \in L$、および$\gamma \in \Gamma$の場合。 命題 VIII、p. 315 の 12 は、代数 $\mathbf{A}[\mathscr{E}; L]$ から C までの準同型 $f$ を与えます。 代数 $\mathbf{A}[\mathscr{E}; L]$ は単純なので、準同型 $f$ は単射法です。 代数 C と $\mathbf{A}[\mathscr{E}; L]$ は K に対して同じ次元を持っているため、$f$ は同型です。

#### 注意 1 {#alg-viii-s16-n10-rem-1 .statement tag=00JN}

L が K 上のエタール代数で、G が L の自己同型群である場合、代数 $\mathbf{A}[\mathscr{E}; L]$ が中心単純であるとは必ずしも当てはまりません (たとえば、$L = K^n$ と $G =\mathfrak{S}_n$ を取ることができます)。

#### 注意 2 {#alg-viii-s16-n10-rem-2 .statement tag=00JO}

次のように、有限ガロア拡大 L と群 G によって代数分裂に関連付けられた 2 共サイクル $c$ 計算するを作成できます。まず、$[A : K] =m^2$ である K 準同型性 $\varphi : A\rightarrow \mathbf{M}_m$(L) が存在します。 $g\in G$ について、$\varphi^g$ を $a\mapsto \varphi (g^{-1}ag)$ で与えられる A から $\mathbf{M}_m(L)$ までの準同型とします。スコーレム・ネーター 定理 (VIII, p. 256, 定理 3) により、$g\in G$ ごとに、$\mathbf{G}\mathbf{L}_m(L)$ のうち元 $u_g$ が存在します。

$$
\varphi^g(a) =u_g\varphi (a)u^{-1}_g
$$

$a\in A$の場合。それでは、集合

$$
c(g, g') =u_gu_{g'}u^{-1}_{gg'}
$$

$\varphi :$ を使用して、G の定義する拡大を $L^*$ で求めることもできます。$g\in G$ が存在する $\gamma$ の群 $\Gamma \subset \mathbf{G}\mathbf{L}_m(L)$ からなるを考慮します。

$$
\varphi^g(a) =\gamma \varphi (a)\gamma^{-1}
$$

$a\in A$ごとに。この拡大の類は、Br(L$/K$)のAの類のΨによる逆像です。

#### 系 {#alg-viii-s16-n10-cor-1 .statement tag=00JP}

写像 $\Phi_{L/K}= \Theta \circ \Psi^{-1}$ 定義する群同型 Br(L$/K$) から $H^2(G,L^*)$ まで。

$K'$ を K の拡大と K-代数の $\varphi : K'\rightarrow L$ 射とします。 G の元 $h$ の集合 H は、 $\lambda (h)\circ \varphi =\varphi$ が G の部分群であり、H に対して $\lambda$ の制限が付与された $K'$-代数 L はガロア代数を超えます$K'$。

#### 命題 14 {#alg-viii-s16-prop-14 .statement tag=00JQ}

次の図式が通勤しています:

Br(L$/K$)$^{\Phi_{L/K}}/$/ $H_2(G,L_*)$

$r_{K'/K}$ 回答$^G_H$

Br(L$/K'$)$^{\Phi_{L/K'}}/$/ $H_2(H,L_*)$ .

This follows from Propositions 7 of VIII, p. 299 and 13 of VIII, p. 317.

### 11. 添字と指数

#### 定理 6 {#alg-viii-s16-thm-6 .statement tag=00JR}

Kを可換体、AをK上の有限次数の中心単純A-代数とする。Lを有限次数のKの分離拡大、つまり代数Aの分解体とする。すると、[L:K][A]は零となるBr(K)。

Lの拡大M、つまり有限次数のKのガロア拡大(V, §10, No. 1、p. 57、命題2)が存在します。 K 属するから部分群 Br(M$/K$) のブラウアー群における A の類 [A]。 G を K 上の M のガロア群とし、$\alpha$ を $H^2(G,M^*)$ (VIII, p. 321, 系) の [A] の像とします。 H を L 以上の M のガロア群とします。すると、H は G の添字 [L : K] の部分群になります (V, §10, No. 7, p. 68, 系 5)。 Res$^G_H(\alpha ) = \Phi_{M/L}(A_{(L)})$ (命題 14) なので、Res$^G_H(\alpha ) = 0$ になります。 VIII, p. 303 の命題 8 により、$[L : K]\alpha = 0$ となり、結果として [L : K][A] = 0 となります。

K を可換体とし、A を K 上の有限次数の中心単純代数とします。 このとき、A は形 $\mathbf{M}_n$(D) の代数と同型であり、D は体と中心 K、および Br(K) の [A] = [D] です。 D の縮小された次数は A のみに依存します。 これを A の縮小次数添字と呼びます。 割るの添字は A の次数を減じたものです。 A の指数は、K のブラウアー群における A の類の位数です。

#### 系 1 {#alg-viii-s16-thm-6-cor-1 .statement tag=00JS}

有限次数の中央の単純代数の指数が可換体割るの添字になります。

これを、中心 K に対する有限次数の体 D について証明するだけで十分です。L を D の最大可換部分体、つまり K の分離拡大とします。 $[D : K] = [L : K]^2$ (VIII、p. 265、系 2、b)、c)) があります。すると、K の拡大 L は、代数 D (VIII, p. 281, 命題 5) の分解体となり、D の次数を減じた [L : K] 一致するとなります。 定理を適用する 6.

#### 系 2 {#alg-viii-s16-thm-6-cor-2 .statement tag=00JT}

K を可換体とし、A を K 上の有限次数の中心単純代数とする。$p$ を素数数とする。 A の $p$ 割る添字の場合、A の割る指数になります。

素数数 $p$ が A の割る指数ではないと仮定し、素数割るが添字ではないことを証明しましょう。 この結果は、A が体の場合に証明すれば十分です。 L を有限次数の K のガロア拡大と分裂 A とします。 G を K 上の L のガロア群とし、H を G の Sylow $p$ 部分群 (I, §6, No. 6, p. 78) とする。 H の不変量の L の $L'= L^H$ 部分体で表します。 $A_{(L')}$ 割るの指数は A の$p$ に対して素数です。 定理 6 までに、$L'$ のブラウアー群に $[L : L'][A_{(L')}] = 0$ ができます。 $[A_{(L')}] = 0$ と体 $L'$ 分裂 A が続きます。 次に、VIII の 2 を系を適用する、p. 283 とします。従って、割る $[L': K]$ の添字となり、従って $p$ では割り切れません。

#### 系 3 {#alg-viii-s16-thm-6-cor-3 .statement tag=00JU}

$p$ を素数数とし、K を標数 $p$ の完全体とします。 A を K 上の有限次数の中心単純代数とします。すると、$p$ は A の割る添字ではありません。

Let us prove that the Brauer group of K does not contain any element of order $p$. 有限次数の K のすべてのガロア拡大 M は完全体 (V, §7, No. 1、p. 36、命題 2) です。 従って、$p$ 番目の冪を取ると、群 $M^*$ の自己同型になります。 従って、$p$による乗法は、Br(M$/K$)と同型である群$H^2$(Gal(M$/K$)$,M^*$)の自己同型となる。

従って、[A] の位数は $p$ に対して素数であり、系 2 によって、その添字は $p$ で割り切れません。

#### 注意 {#alg-viii-s16-n11-rem-1 .statement tag=00JV}

四元数代数のテンソル積を考慮すると、中心 K、指数 2、および任意に大きい添字 (cf. VIII、p. 371、練習問題 7 と 8) で構成する体が可能です。

$*$逆に、K が有限体上の $p$ 進数体の有限ガロア拡大または形式冪系列の体である場合、K 上の有限次数の中心単純代数の指数は次のようになります。 添字 (VIII, p. 332, 練習問題 17, e)) に等しい。$*$

### 練習問題 {#alg-viii-s16-exercises}

[§ 16 に対して練習問題](exercises/s16/)を参照してください。
