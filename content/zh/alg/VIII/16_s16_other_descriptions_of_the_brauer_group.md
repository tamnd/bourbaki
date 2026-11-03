---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 16
section_title: Other Descriptions of the Brauer Group
lang: zh
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
content_sha256: c04eb2767f09dd7abd30f323ce594de74f233606d5fe0f02d94810e19f3274b3
translated_from: content/en/alg/VIII/16_s16_other_descriptions_of_the_brauer_group.md
translation_method: google
source_content_sha256: 67633b439572bf5a4dcc4c35edb70b8c99883cdac1bfa5ce829e7e8f5be14d83
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-1fd6073a
glossary_version: 34
glossary_terms_sha256: 0beceb57035d49ee3eda89378692ac98b5052acade8a28c54a22bb3855fcea12
prompt_sha256: 8cbde7b7ea18274bea5720e1f500823a36194a717a2895a9c9e7e3ffc4a3a3ae
---

## § 16。 布劳尔群的其他描述

在这个截面中，如果F是F的阿贝尔的群和$g$自同构，那么我们将$g(f)$写成$g\cdot f$。

### 1. $\tau$-群的扩展

在这个小节中，我们将群G，阿贝尔的群F固定为乘法，并将群同态$\tau$从G到F的自同构群Aut(F)。我们用$e$表示G的单位元素， F 的单位元素除 1。

回想一下 (I, §6, No. 1, p. 65)，F 的 G 的扩张 $\mathscr{E}$ 是三元组 $(\Gamma , \iota , \pi )$，其中 Γ 是群，$\pi : \Gamma \rightarrow G$ 是满同态，$\iota$ 是单同态，从 F 到 Γ 使得我（$\iota$）$=$克尔（$\pi$）。让$\mathscr{E}= (\Gamma , \iota , \pi )$成为扩张。对于每个 $\gamma \in \Gamma$、映射 $\varphi_{\gamma}: F\rightarrow F$ 定义

$$
\iota (\varphi_{\gamma}(f)) =\gamma \iota (f)\gamma^{-1}
$$

对于 $f\in F$ 是 F 的自同构。由于 F 是可交换的，对于每个 $f\in F$，由 $\iota (f)$ 定义的自同构是 F 上的恒等映射。通过经过到商，我们得到同态 Int$_{\mathscr{E}}$从 G 到 Aut(F) 的特征为

$\gamma \iota (f)\gamma^{-1}=\iota$(整数$_{\mathscr{E}}(\pi (\gamma ))\cdot f$)

对于 $\gamma \in \Gamma$ 和 $f\in F$。

F 对 G 的$A\tau$-扩展是扩张 $\mathscr{E}= (\Gamma , \iota , \pi )$，使得 Int$_{\mathscr{E}}$ 等于 $\tau$，在其他字中，满足关系

$$
\gamma \iota (f)\gamma^{-1}=\iota (\tau (\pi (\gamma ))\cdot f) \tag{1}
$$

对于 $\gamma \in \Gamma$ 和 $f\in F$。如果$\mathscr{E}= (\Gamma , \iota , \pi )$和$\mathscr{E}'= (\Gamma ', \iota ', \pi ')$是$\tau$扩展，则从$\mathscr{E}$到$\mathscr{E}'$的$\tau$扩展中的态射是从$\mathscr{E}$到扩张的态射 $\mathscr{E}'$（I, §6, No. 1，p. 65），即群同态$u: \Gamma \rightarrow \Gamma '$，使得$\pi '\circ u=\pi$和$\iota '=u\circ \iota$。请注意，$\tau$-扩展形式结构种，其中每个态射是同构（集合理论、IV, §1, No. 5、p. 264和I, §6, No. 1， p. 66，命题1)。用 Iso$_{\tau}(\mathscr{E},\mathscr{F})$ 关系表示

“$\mathscr{E}$和$\mathscr{F}$是同构的$\tau$扩展。”

这是等价关系； 扩张 $\mathscr{E}$ 的类是对象的类相当于 Iso$_{\tau}($集合理论、II, §6, No. 6、p. 122 的$\mathscr{E}$）。

#### 引理 1 {#alg-viii-s16-lem-1 .statement tag=00I9}

关系

“$\alpha$ 是 Iso$_{\tau}$ $\tau$ 扩展的类”

$\alpha$ 中有集合化。

集合$E_0= F\times G$，并考虑映射$\iota_0: F\rightarrow E_0$和$\pi_0: E_0\rightarrow G$由$\iota_0(f) = (f, e)$定义为$f\in F$和$\pi_0(f, g) =g$定义为$(f, g)\in F\times G$。令 $\mathscr{E}= (\Gamma , \iota , \pi )$ 为 G 由 F 的 $\tau$ 扩展。 映射 $\pi$ 是满射，因此有截面 $\sigma : G\rightarrow \Gamma$ 使得 $\sigma (e) =e$。从 $F\times G$ 到 Γ 的映射 $u: (f, g)\mapsto \iota (f)\sigma (g)$ 是双射的。我们将通过结构转账获得的群运算赋予$F\times G$。那么三元组$(E_0, \iota_0, \pi_0)$是与$\mathscr{E}$同构的$\tau$扩展。 引理 1 现在源自集合理论、II, §6, No. 6、p. 122。

我们用$\tau$的类的Ex$_{\tau}(G,F)$集合-关系Iso$_{\tau}$的扩展来表示。

#### 例 1 {#alg-viii-s16-n1-exa-1 .statement tag=00IA}

外部半直积 $(F\times_{\tau}G, i, p)$ (I, §6, No. 1、p. 66、命题 3) 是 $\tau$ 扩展；我们用$\mathscr{I}_{\tau}$表示。如果 $\tau$ 扩展与 $\tau$ 扩展 $\mathscr{I}_{\tau}$ 同构，我们就说它是半平凡的。

#### 例 2 {#alg-viii-s16-n1-exa-2 .statement tag=00IB}

对于$i\in  \{1,2\}$，从$G_i$到$F_i$的自同构群取群$G_i$、阿贝尔的群$F_i$、群同态$\tau_i$。我们用 $\tau_1\times \tau_2: G_1\times G_2\rightarrow$ Aut(F$_1\times F_2$) 同态定义为

$$
(\tau_1\times \tau_2)(g_1, g_2)\cdot (f_1, f_2) = (\tau_1(g_1)\cdot f_1, \tau_2(g_2)\cdot f_2)
$$

对于 $g_1\in G_1,g_2\in G_2,f_1\in F_1$ 和 $f_2\in F_2$。令$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$为$G_1$经$F_1$的$\tau_1$延伸，$\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$为$G_2$经$F_2$的$\tau_2$延伸。那么三元组$(\Gamma_1\times \Gamma_2, \iota_1\times \iota_2, \pi_1\times \pi_2)$是$G_1\times G_2$的$\tau_1\times \tau_2$扩展$F_1\times F_2$；称为扩张、$\mathscr{E}_1$和$\mathscr{E}_2$的外乘积，记为$\mathscr{E}_1\times \mathscr{E}_2$。

### 2. $\tau$-扩展的逆像

令 G 和$G'$ 为群。令 F 为阿贝尔的群，并令 $\tau : G\rightarrow$ Aut(F) 和 $u: G'\rightarrow G$ 为群同态。考虑群同态$\tau '=\tau \circ u: G'\rightarrow$Aut(F)，并用$\Gamma '$表示相对于$\pi$和$u$的纤维乘积$\Gamma \times_GG'$（I, §4, No. 8，p. 46）。 对$(\gamma , g')$$\Gamma \times G'$由……组成子群使得$\pi (\gamma ) =u(g')$。令$\iota ': F\rightarrow \Gamma '$为群同态，由$\iota '(\alpha ) = (\iota (\alpha ), e)$对$\alpha \in F$给出，并用$\pi ': \Gamma '\rightarrow G'$表示第二个投影。那么态射$\iota '$是单射，态射$\pi '$是满射，因为$\pi$是，$\iota '$重合的像和$\pi '$的核。此外，对于每个$\alpha \in F$和$\gamma '= (\gamma , g)\in \Gamma '$，我们有关系

$$
\gamma '\iota '(\alpha )\gamma^{'-1}= (\gamma , g)(\iota (\alpha ), e)(\gamma , g)^{-1}= (\iota (\tau (\pi (\gamma )).\alpha ), e) =\iota '(\tau '(\pi '(\gamma ')).\alpha )
$$

因而，$(\Gamma ', \iota ', \pi ')$是F对$G'$的$\tau '$扩展；我们用$u$来称呼它为$\mathscr{E}$的逆像，并用$u^*(\mathscr{E})$来表示。第一个投影是群同态 $\varphi : \Gamma '\rightarrow \Gamma$，我们称之为规范。

#### 命题 1 {#alg-viii-s16-prop-1 .statement tag=00IC}

以下图表通勤：

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

(2)

$\varphi u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

此外，如果$\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$是$\tau '$扩展且$\varphi_1: \Gamma '_1\rightarrow \Gamma$是群同态，使得图表

F $^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G

通勤，那么存在$\tau '$的唯一态射$\psi$-从$\mathscr{E}_1'$到$u^*(\mathscr{E})$的延伸，这样我们就有$\varphi_1=\varphi \circ \psi$。

第一个图表的交换律源自$\varphi$的定义。 $\psi$的存在和唯一性由下面的引理2得出。

#### 引理 2 {#alg-viii-s16-lem-2 .statement tag=00ID}

令 $F'_1$ 为阿贝尔的群，并令 $w: F'_1\rightarrow$ F 和 $\tau_1: G'\rightarrow$ Aut(F$'_1$) 为群同态，使得

$$
w(\tau_1(g)(f)) =\tau (u(g))(w(f))
$$

对于每个$f\in F'_1$和$g\in G'$。令$\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$是$G'$通过$F'_1$和$\varphi_1: \Gamma '_1\rightarrow \Gamma$群同态的$\tau_1$扩展，使得以下图表可通勤：

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'$

$w\varphi_1u$

F $^{\iota}$ // Γ $^{\pi}$ // G.

那么存在唯一群同态$\psi : \Gamma '_1\rightarrow \Gamma '$使得图表

${F'_1}^{\iota'_1}$ // ${\Gamma'_1}^{\pi_1'}$ // $G'$

$w\psi$

F $^{\iota'}$ // ${\Gamma'}^{\pi'}$ // $G'$

通勤和$\varphi_1=\varphi \circ \psi$。

如果群同态 $\psi : \Gamma '_1\rightarrow \Gamma '$ 具有所需的属性，则满足关系

$$
\psi (\gamma ) = (\varphi \circ \psi (\gamma ), \pi '\circ \psi (\gamma )) = (\varphi_1(\gamma ), \pi '_1(\gamma ))
$$

每$\gamma \in \Gamma '_1$。相反，由$\gamma \mapsto (\varphi_1(\gamma ), \pi_1'(\gamma ))$定义的从$\Gamma '_1$到$\Gamma \times G'$的群同态在纤维乘积$\Gamma \times_GG'$中有值，因为每个$\gamma \in \Gamma '_1$都有$\pi \circ \varphi_1(\gamma ) =u\circ \pi_1'(\gamma )$。

#### 推论 1 {#alg-viii-s16-lem-2-cor-1 .statement tag=00IE}

令$\mathscr{E}_1$和$\mathscr{E}_2$为$\tau$-G通过F的扩展，并令$\psi$为$\tau$的态射-从$\mathscr{E}_1$到$\mathscr{E}_2$的扩展。用 $\varphi_1($resp 表示。 $\varphi_2)$典范同态对应$u^*(\mathscr{E}_1) ($。 $u^*(\mathscr{E}_2))$。那么存在$\tau '$的唯一态射-从$u^*(\mathscr{E}_1)$到$u^*(\mathscr{E}_2)$的延伸，记为$u^*(\psi )$，使得$\varphi_2\circ u^*(\psi ) =\psi \circ \varphi_1$。

应用命题1至$\psi \circ \varphi_1$就足够了。

因此，$\tau '$扩展$u^*(\mathscr{E})$的类仅取决于$\mathscr{E}$的类。我们还用 $u^*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G',F)$ 映射表示，将$\tau$扩展名$\mathscr{E}$的类发送到$\tau '$扩展名$u^*(\mathscr{E})$的类。

#### 推论 2 {#alg-viii-s16-lem-2-cor-2 .statement tag=00IF}

令$u': G''\rightarrow G'$为群同态，并令$\mathscr{E}$为F对G的$\tau$扩展。集合$\tau ''=\tau '\circ u'$，并分别用$\varphi ($表示。 $\varphi ',\varphi '')$ 典范同态与 $\tau '$ 扩展名 $u^*(\mathscr{E}) ($resp 相关。 $\tau ''$-扩展名$u^{'*}(u^*(\mathscr{E}))$，$\tau ''$-扩展名$(u\circ u')^*(\mathscr{E}))$。那么从$\tau ''$扩展$u^{'*}(u^*(\mathscr{E}))$到$\tau ''$扩展$(u\circ u')^*(\mathscr{E})$存在唯一态射$\psi$，使得$\varphi ''\circ \psi =\varphi \circ \varphi '$。

#### 例 {#alg-viii-s16-n2-exa-1 .statement tag=00RI}

令 H 为 G 的子群和 $j: H\rightarrow G$ 典范嵌入。那么对于每个$\tau$-扩展$\mathscr{E}= (\Gamma , \iota , \pi )$，$\tau \circ j$-扩展$j^*(\mathscr{E})$与$(\overset{-1}{\pi}(H), \iota ', \pi ')$同构的，其中$\iota ': F\rightarrow \overset{-1}{\pi}(H)$（或$\pi ':\overset{-1}{\pi}(H)\rightarrow H$）是群同态$f\mapsto \iota (f)$（或$\gamma \mapsto \pi (\gamma )$）。更一般地，如果群同态 $u: G'\rightarrow G$ 是单射，则典范同态 $\varphi$ 与像 $\overset{-1}{\pi}(u(G'))$ 是单射。

### 3. $\tau$-扩展的直接像

令G为群，令F和$F'$为阿贝尔的群，令$\tau$（或$\tau '$）为从G到F的自同构群（或$F'$）的群同态，并令$v: F\rightarrow F'$为群同态这样

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{3}
$$

对于每个$g\in G$和$f\in F$。令$\mathscr{E}= (\Gamma , \iota , \pi )$为F对G的$\tau$扩展。令$\widetilde{\Gamma}$为外部半直积$F'\times_{\tau'\circ\pi}\Gamma$。我们用$\widetilde{\imath}: F'\rightarrow \widetilde{\Gamma}$同态$f\mapsto (f, e)$表示，并用$\widetilde{p}:\widetilde{\Gamma}\rightarrow \Gamma$表示第一个投影。令 $j: F\rightarrow \widetilde{\Gamma}$ 为由 $f\mapsto (v(f), \iota (f)^{-1})$ 定义的映射。由于$\iota$的像包含在$\tau '\circ \pi$的核中，所以映射$j$是群同态；它是单射的，因为 $\iota$ 是单射的。我们有关系

$$
(f', \gamma )j(f)(f', \gamma )^{-1}= (f', \gamma )(v(f), \iota (f)^{-1})(f', \gamma )^{-1}
$$

$$
= (\tau '(\pi (\gamma ))\cdot v(f), \iota (\tau (\pi (\gamma ))\cdot f)^{-1}) \tag{4}
$$

$$
=j(\tau (\pi (\gamma ))\cdot f)
$$

对于$f\in F,\gamma \in \Gamma$和$f'\in F'$。因而，$j$的像是$\widetilde{\Gamma}$的正常子群。我们用$j$的像来表示$\widetilde{\Gamma}$的$\Gamma '$商。我们用$\widetilde{\Gamma}$到$\Gamma '$和$\widetilde{\imath}$的典范满射中的$\iota '$合成来表示。 同态$\pi \circ \widetilde{p}$中的核是乘积$F'\times \iota$(F)，其中$j$中的包含像。我们将定义$\pi ': \Gamma '\rightarrow G$作为群同态从$\pi \circ \widetilde{p}$推导出经过到商。由于$\iota$是单射的，$j(F)$和$\widetilde{\imath}(F')$的交减少为$\widetilde{\Gamma}$的单位元素；由此可见 $\iota '$ 是单射的。 映射从 $F'\times F$ 到 $F'\times \iota (F) =$ Ker($\pi \circ \widetilde{p}$) 给出

$$
(f', f)\longmapsto (f'v(f), \iota (f)^{-1})
$$

是群同构。 像 $\iota '$ 因此重合核 $\pi '$。由于 $\pi$ 和 $\widetilde{p}$ 是满射，所以 $\pi '$ 也是满射。这证明$\mathscr{E}'= (\Gamma ', \iota , \pi ')$是G的$\tau '$扩展$F'$；我们用$v$来称呼它为$\mathscr{E}$的直接像，并用$v_*(\mathscr{E})$来表示。由$\gamma \mapsto (1, \gamma )$给出的典范满射从$\widetilde{\Gamma}$到$\Gamma '$和群同态从$\widetilde{\Gamma}$的合成是我们称之为规范的群同态$\varphi : \Gamma \rightarrow \Gamma '$。

#### 命题 2 {#alg-viii-s16-prop-2 .statement tag=00IG}

在上面的记号中，以下图表通勤：

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{5}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

令 $\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi_1')$ 为 G $F'$ 的 $\tau '$ 扩展，并令 $\varphi_1: \Gamma \rightarrow \Gamma '_1$ 为群同态，使得以下图表可通勤：

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // G.

那么存在$\tau '$的唯一态射$\psi$-从$v_*(\mathscr{E})$到$\mathscr{E}_1'$的扩展，这样我们就有$\varphi_1=\psi \circ \varphi$。

第一个图表的交换律之后是构造。 $\psi$的存在性和唯一性由下面的引理3得出。

#### 引理 3 {#alg-viii-s16-lem-3 .statement tag=00IH}

令$G'_1$为群，并令$w: G\rightarrow G'_1$和$\tau_1: G'_1\rightarrow$Aut(F$'$)为群同态，使得$\tau '=\tau_1\circ w$。令$\mathscr{E}_1'= (\Gamma '_1, \iota '_1, \pi '_1)$为$G'_1$通过$F'$的$\tau_1$扩展，并令$\varphi_1: \Gamma \rightarrow \Gamma '_1$为群同态，使得以下图表可通勤：

F $^{\iota}$ // Γ $^{\pi}$ // G

$v\varphi_1w$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$。

那么存在唯一群同态$\psi : \Gamma '\rightarrow \Gamma '_1$使得图表

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G

$\psi w$

${F'}^{\iota'_1}$ // ${\Gamma'_1}^{\pi'_1}$ // $G'_1$ 通勤和 $\varphi_1=\psi \circ \varphi$。

对于任何$(f, \gamma )\in F'\times \Gamma$，用$(f, \gamma )$表示$\Gamma '$中$(f, \gamma )$的类。如果群同态 $\psi : \Gamma '\rightarrow \Gamma '_1$ 具有所需的性质，则满足关系

$$
\psi (f', \gamma )=\psi (\iota '(f')\varphi (\gamma )) =\iota '_1(f')\varphi_1(\gamma )
$$

对于每个$f'\in F'$和$\gamma \in \Gamma$。相反，由$(f, \gamma )\mapsto \iota '_1(f)\varphi_1(\gamma )$给出的从$F'\times_{\tau'\circ\pi}\Gamma$到$\Gamma '_1$的映射$\widetilde{\psi}$是群同态。确实，我们有关系

$$
\iota '_1(f)\varphi_1(\gamma )\iota '_1(f')\varphi_1(\gamma ') =\iota '_1(f \tau_1(\pi '_1(\varphi_1(\gamma )))\cdot f')\varphi_1(\gamma \gamma ')
$$

$$
=\iota '_1(f \tau '(\pi (\gamma ))\cdot f')\varphi_1(\gamma \gamma ')
$$

对于 $f, f'\in F'$ 和 $\gamma , \gamma '\in \Gamma$。 $\widetilde{\psi}$ 的核包含 $j$ 的图像，因为 $\iota '_1(v(f)) =\varphi_1(\iota (f))$ 对于 $f\in F$，并且通过传递给商从 $\widetilde{\psi}$ 推导出的态射 $\psi$ 具有所需的属性。

#### 注 {#alg-viii-s16-n3-rem-1 .statement tag=00II}

用 $\tau '$ 扩展的 Σ 结构种表示，并且定义 $\alpha$-映射为从 Γ 到群 $\Gamma '$ 的映射，底层为 $\tau '$ 扩展，为群同态并进行以下图表交换：

F $^{\iota}$ // Γ $^{\pi}$ // G

$$
v\varphi \tag{6}
$$

${F'}^{\iota'}$ // ${\Gamma'}^{\pi'}$ // G .

命题2表示$v_*(\mathscr{E})$是相应的普遍映射问题(集合理论、IV, §3, No. 1、p. 284)中的解。

#### 推论 1 {#alg-viii-s16-lem-3-cor-1 .statement tag=00IJ}

令$\mathscr{E}_1$和$\mathscr{E}_2$为$\tau$-G通过F的扩展，并令$\psi$为$\tau$的态射-从$\mathscr{E}_1$到$\mathscr{E}_2$的扩展。分别用 $\varphi_1($ 表示。 $\varphi_2)$ 典范同态分别为 $v_*(\mathscr{E}_1) ($。 $v_*(\mathscr{E}_2))$。那么存在$\tau '$的唯一态射-从$v_*(\mathscr{E}_1)$到$v_*(\mathscr{E}_2)$的延伸，记为$v_*(\psi )$，使得$\varphi_2\circ \psi =v_*(\psi )\circ \varphi_1$。

应用命题2至$\varphi_2\circ \psi$就足够了。

因此，$\tau '$扩展$v_*(\mathscr{E})$的类仅取决于$\mathscr{E}$的类。我们还用 $v_*:$ Ex$_{\tau}(G,F)\rightarrow$ Ex$_{\tau'}(G,F')$ 映射来表示，将$\tau$扩展名$\mathscr{E}$的类发送到$\tau '$扩展名$v_*(\mathscr{E})$的类。

#### 推论 2 {#alg-viii-s16-lem-3-cor-2 .statement tag=00RJ}

我们保留命题中的记号。令 $F''$ 为阿贝尔的群，并令 $\tau '': G\rightarrow$ Aut(F$''$) 和 $v': F'\rightarrow F''$ 为群同态，使得

$$
\tau ''(g)\cdot v'(f) =v'(\tau '(g)\cdot f)
$$

对于 $g\in G$ 和 $f\in F'$。令 $\mathscr{E}$ 为 G 由 F 的 $\tau$ 扩展，并用 $\varphi ($resp 表示。 $\varphi ',\varphi '')$ 典范同态与 $v_*(\mathscr{E}) ($resp 相关。 $v'_*(v_*(\mathscr{E}))$，$(v'\circ v)_*(\mathscr{E}))$。那么存在从G的$\tau ''$扩展$v'_*(v_*(\mathscr{E}))$经$F''$到$\tau ''$扩展$(v'\circ v)_*(\mathscr{E})$的唯一态射$\psi$，使得$\varphi ''=\psi \circ \varphi '\circ \varphi$。

#### 例 1 {#alg-viii-s16-n3-exa-1 .statement tag=00IK}

令$j:\{1\} \rightarrow F$为典范嵌入。半平凡扩张 $\mathscr{I}_{\tau}$ 同构于 $j_*((G, i$，Id$_G))$，其中 $i:\{e\} \rightarrow G$ 是典范嵌入。令$c: F\rightarrow F$为常数同态$f\mapsto 1$，并令$\mathscr{E}$为$\tau$扩展。 $\tau$扩展名$c_*(\mathscr{E})$也与$\mathscr{I}_{\tau}$同构的。

#### 例 2 {#alg-viii-s16-n3-exa-2 .statement tag=00IL}

设 E 为 F 的子群在 G 的作用下稳定。用 E 的 F 的 $F'$ 商表示，用 $v: F\rightarrow F'$ 典范同态表示，并用 $\tau ': G\rightarrow$ Aut(F$'$) 作用在 $F'$ 上表示，其特征为

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

对于 $g\in G$ 和 $f\in F$。令 $\mathscr{E}= (\Gamma , \iota , \pi )$ 为 G 通过 F 的 $\tau$ 扩展。那么 $\iota (E)$ 是 Γ 的正规子群，并且 G 通过 $F'$ 的 $\tau '$ 扩展 $v_*(\mathscr{E})$ 同构于扩张 $(\Gamma /\iota (E), \iota , \pi )$，其中$\overline{\iota}$和$\overline{\pi}$是群同态从$\iota$和$\pi$推出经过到商。由此同构、典范同态$\varphi$与$v_*(\mathscr{E})$对应到典范同态从$\Gamma /\iota (E)$相关联。

#### 命题 3 {#alg-viii-s16-prop-3 .statement tag=00IM}

设G和$G'$为群，设F和$F'$为阿贝尔的群。令 $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$)$,u: G'\rightarrow G$，且 $v: F\rightarrow F'$ 为群同态，使得

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

对于 $g\in G$ 和 $f\in F$。我们写$\tau ''=\tau '\circ u$。令 $\mathscr{E}$ 为 F 的 G $\tau$ 扩展。我们用 $\varphi_u($resp 表示。 $\varphi_v,\varphi '_u,\varphi '_v)$ 典范同态相应的至 $\tau \circ u$ 分机 $u^*(\mathscr{E}) ($resp。 $\tau '$-分机 $v_*(\mathscr{E})$、$\tau ''$-分机 $u^*(v_*(\mathscr{E}))$ 和 $v_*(u^*(\mathscr{E})))$。那么存在$\tau ''$的唯一态射$\psi$-从$v_*(u^*(\mathscr{E}))$到$u^*(v_*(\mathscr{E}))$的延伸，使得$\varphi_v\circ \varphi_u=$$\varphi '_u\circ \psi \circ \varphi '_v$。

我们用$(\Gamma_u, \iota_u, \pi_u)$（或$(\Gamma '_u, \iota '_u, \pi '_u)$）表示$\tau \circ u$扩展名$u^*(\mathscr{E})$（或$\tau ''$扩展名$u^*(v_*(\mathscr{E}))$）。 应用引理 2 of VIII, p. 287 to $\varphi_v\circ \varphi_u$，我们发现存在群同态 $\psi_1: \Gamma_u\rightarrow \Gamma '_u$使得图表

F $^{\iota_u}$ // $\Gamma_u^{\pi_u}$ // $G'$

$v\psi_1$

${F'}^{\iota'_u}$ // ${\Gamma'_u}^{\pi'_u}$ // $G'$

通勤和$\varphi '_u\circ \psi_1=\varphi_v\circ \varphi_u$。 $\psi$ 的存在源自于命题 2 应用于$\psi_1$。相反，如果 $\psi '$ 也具有所需的属性，则我们有 $\psi '\circ \varphi '_v=\psi_1$ × 引理 2，因此 $\psi '=\psi$ (命题 2)。

### 4. 群运算 on 类 of $\tau$-扩展

设G为群，F为阿贝尔的群，$\tau : G\rightarrow$Aut(F)为群同态。我们用$\delta : G\rightarrow G\times G$表示对角线映射$g\mapsto$$(g, g)$和$m: F\times F\rightarrow F$乘法同态$(f_1, f_2)\mapsto$$f_1f_2$。我们用 $s: F\rightarrow F$ 群同态表示，$f\mapsto f^{-1}$ 给出。令$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$和$\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$为$\tau$-G通过F的扩展。因为我们有关系

$$
m(((\tau \times \tau )\circ \delta )(g)\cdot (f_1, f_2)) =\tau (g)\cdot m(f_1, f_2)
$$

对于每个$g\in G$和所有$f_1, f_2\in F$，扩张$m_*(\delta^*(\mathscr{E}_1\times \mathscr{E}_2))$是$\tau$扩展；我们称其为$\tau$扩展$\mathscr{E}_1$和$\mathscr{E}_2$的乘积，并用$\mathscr{E}_1\mathscr{E}_2$表示。这个扩张的类仅取决于扩张$\mathscr{E}_1$和$\mathscr{E}_2$类（VIII，p. 288，推论1和VIII，p. 291， 推论1)。因此，这给出了 Ex$_{\tau}(G,F)$ 上的合成的律。

#### 注 {#alg-viii-s16-n4-rem-1 .statement tag=00IN}

令$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$和$\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$为F对G的$\tau$扩展。令$\mathscr{E}_1\mathscr{E}_2= (\Gamma , \iota , \pi )$为这些扩张的乘积。继VIII、p. 289、构造的例给出从纤维乘积$\Gamma_1\times_G\Gamma_2$到核是群同态的像的满射群同态 $f\mapsto (\iota_1(f), \iota_2(f)^{-1})$从F到$\Gamma_1\times_G\Gamma_2$。

#### 命题 4 {#alg-viii-s16-prop-4 .statement tag=00IO}

$\tau$的乘积扩展赋予集合Ex$_{\tau}(G,F)$与阿贝尔的群的结构。它的单位元素是半平凡的扩张$\mathscr{I}_{\tau}$的类。 $\tau$扩展$\mathscr{E}$的类的倒数是$s_*(\mathscr{E})$的类。

律的结合性源自图表的交换律

$$
\begin{array}{ccc}
G & \xrightarrow{\delta} & G \times G \\
\downarrow \delta & & \downarrow \operatorname{Id} \times \delta \\
G \times G & \xrightarrow{\delta \times \operatorname{Id}} & G \times G \times G
\end{array}
$$
和
$$
\begin{array}{ccc}
F \times F \times F & \xrightarrow{m \times \operatorname{Id}} & F \times F \\
\downarrow \operatorname{Id} \times m & & \downarrow m \\
F \times F & \xrightarrow{m} & F
\end{array}
$$

以及从推论 2 / VIII、p. 288； 推论 2 个VIII、p. 291；以及 VIII、p. 292 中的命题 3 个。

令 $\Delta : F \to F \times F$ 为对角线映射 $f \mapsto (f, f)$。令 $\mathscr{E} = (\Gamma, \iota, \pi)$ 为 $\tau$ 扩展。令 $\tilde{\Delta} : \Gamma \to \Gamma \times_G \Gamma$ 为由 $\gamma \mapsto (\gamma, \gamma)$ 给出的群同态。以下图表通勤：

$$
\begin{array}{ccccc}
F & \xrightarrow{\iota} & \Gamma & \xrightarrow{\pi} & G \\
\downarrow \Delta & & \downarrow \tilde{\Delta} & & \parallel \\
F \times F & \longrightarrow & \Gamma \times_G \Gamma & \longrightarrow & G.
\end{array}
$$

由VIII、p. 290的命题 2，可知$(\tau \times \tau) \circ \delta$扩展$\delta^*(\mathscr{E} \times \mathscr{E})$与$\Delta_*(\mathscr{E})$同构的。

用 $c : F \to F$ 表示常数同态 $f \mapsto 1$。通过VIII、p. 292的例 1，对于合成的律，$\mathscr{I}_\tau$是单位元素，这一事实是从同构从$\delta^*(\mathscr{E} \times \mathscr{E})$到$\Delta_*(\mathscr{E})$得出的，并且交换律图表

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times c) \circ \Delta} & F \times F \\
(c \times \operatorname{Id}_F) \circ \Delta & & \downarrow \operatorname{Id}_F \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

最后一个断言由交换律图表推出

$$
\begin{array}{ccc}
F & \xrightarrow{(\operatorname{Id}_F \times s) \circ \Delta} & F \times F \\
(s \times \operatorname{Id}_F) \circ \Delta & & \downarrow c \\
& & \downarrow m \\
F \times F & \xrightarrow{m} & F.
\end{array}
$$

令$\mathscr{E}_1 = (\Gamma_1, \iota_1, \pi_1)$和$\mathscr{E}_2 = (\Gamma_2, \iota_2, \pi_2)$为$\tau$扩展。 群同构 $\Gamma_1 \times \Gamma_2 \to \Gamma_2 \times \Gamma_1$ 由 $(\gamma_1, \gamma_2) \mapsto (\gamma_2, \gamma_1)$ 限制至群同构 $\sigma : \Gamma_1 \times_G \Gamma_2 \to \Gamma_2 \times_G \Gamma_1$ 给出。因为关系

$$
\sigma(\iota_1(f), \iota_2(f)^{-1}) = (\iota_2(f^{-1}), \iota_1(f^{-1})^{-1})
$$

$f\in F$、群同态 $\sigma$ 诱导，由经过至商、$\tau$ 的态射 - 从 $\mathscr{E}_1\mathscr{E}_2$ 延伸至 $\mathscr{E}_2\mathscr{E}_1$。所以合成的律是可交换的。

#### 命题 5 {#alg-viii-s16-prop-5 .statement tag=00IP}

a) 令G和$G'$为群，并令F为阿贝尔的群。令$\tau : G\rightarrow$ Aut(F) 和$u: G'\rightarrow G$ 为群同态。 映射$u^*:$Ex$_{\tau}(G,F)\rightarrow$Ex$_{\tau\circ u}(G',F)$为群同态。

b) 令G为群，令F和$F'$为阿贝尔的群。设 $\tau : G\rightarrow$ Aut(F)$,\tau ': G\rightarrow$ Aut(F$'$)，且 $v: F\rightarrow F'$ 为群同态，使得

$$
\tau '(g)\cdot v(f) =v(\tau (g)\cdot f)
$$

对于 $g\in G$ 和 $f\in F$。 映射$v_*:$Ex$_{\tau}(G,F)\rightarrow$Ex$_{\tau'}(G,F')$为群同态。

这是从图表的交换律得出的

${G'}^{\delta}$ // $G'\times G'F\times F^m$ // F

$_uu_{\times u}$ 和 $v_{\times v}v$

G $^{\delta}$ // $G\times GF'\times {F'}^m$ // $F'$。

### 5. 上同调描述

令G为群，令F为阿贝尔的群，令$\tau : G\rightarrow$Aut(F)为群同态。对于任何$g\in G$和$f\in F$，我们也将$\tau (g)\cdot f$写为$^gf$。 G 的 2-cocycle 与 F 中的值是映射 $c: G\times G\rightarrow F$，这样对于每个 $(g_1, g_2, g_3)\in G\times G\times G$，我们有

$$
g_{_1}c(g_2, g_3)c(g_1, g_2g_3) =c(g_1, g_2)c(g_1g_2, g_3) \tag{7}
$$

由于F是可交换的，2-余循环的集合从$G\times G$到F是映射群子群；我们用$Z^2(G,F)$表示。我们用$C^1(G,F)$表示从G到F的映射的群。对于每个 $h\in C^1(G,F)$ 和 $(g_1, g_2)\in G\times G$，集合

$$
(\partial h)(g_1, g_2) =^{g_1}h(g_2)h(g_1g_2)^{-1}h(g_1) \tag{8}
$$

简单计算可知映射$\partial h: G\times G\rightarrow F$是一个2余循环。 映射$\partial : C^1(G,F)\rightarrow Z^2(G,F)$是群同态。对于任何$h\in C^1(G,F)$，2-余循环$\partial h$称为2-余界。 群$Z^2(G,F)/\partial (C^1(G,F))$用$H^2(G,F)$表示，与F中的系数一起称为G的第二个上同调群。

$*$上述记号与X, §6、n$^o8$、p. 112关于群上同调的一致。$*$

令 $\mathscr{E}= (\Gamma , \iota , \pi )$ 为 $\tau$ 扩展。令 $\sigma$ 为满射映射 $\pi ($集合理论, II, §3, No. 8, p. 86) 的截面，即从 G 到 Γ 的映射，使得 $\pi (\sigma (g)) =g$ 对于每个G 中的$g$。对于每个 $g_1, g_2\in G$，$\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}$ 属于到 Ker($\pi$ )，因此存在唯一映射 $c_{\sigma}: G\times G\rightarrow F$ 使得

$$
\iota (c_{\sigma}(g_1, g_2)) =\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1} \tag{9}
$$

对于所有$g_1, g_2\in G$。当且仅当 $\sigma$ 是群同态时，映射 $c_{\sigma}$ 与值 1 一致。

#### 命题 6 {#alg-viii-s16-prop-6 .statement tag=00IQ}

映射$c_{\sigma}$是群$Z^2(G,F)$的元素，上同调群$H^2(G,F)$中的类仅取决于$\tau$扩展名$\mathscr{E}$的类。

我们说映射$c_{\sigma}$是与$\sigma$相关的2-余循环，并且$H^2(G,F)$中的上同调类是$\tau$扩展$\mathscr{E}$的上同调类。

我们首先验证$c_{\sigma}$满足余循环条件。设$g_1,g_2$和$g_3$为G的元素。使用VIII、p. 285和(9)的公式(1)，我们得到关系

$$
\iota (^{g_1}c_{\sigma}(g_2, g_3)c_{\sigma}(g_1, g_2g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_2g_3)^{-1}\sigma (g_1)^{-1}\sigma (g_1)\sigma (g_2g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

和

$$
\iota (c_{\sigma}(g_1, g_2)c_{\sigma}(g_1g_2, g_3))
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}\sigma (g_1g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

$$
=\sigma (g_1)\sigma (g_2)\sigma (g_3)\sigma (g_1g_2g_3)^{-1}
$$

因此，映射 $c_{\sigma}$ 是 $Z^2(G,F)$ 的元素。

现在让我们证明$H^2(G,F)$中$c_{\sigma}$的像独立于所选的截面$\sigma$。令$\sigma$和$\sigma '$为截面。对于 G 的每个元素 $g$，存在 F 的唯一元素 $a_g$，使得 $\sigma '(g) =\iota (a_g)\sigma (g)$。令$g_1$和$g_2$为G的元素。使用定义(9)，我们得到等式

$$
\iota (c_{\sigma'}(g_1, g_2)) =\sigma '(g_1)\sigma '(g_2)\sigma '(g_1g_2)^{-1}
$$

$$
=\iota (a_{g_1})\sigma (g_1)\iota (a_{g_2})\sigma (g_2)\sigma (g_1g_2)^{-1}\iota (a_{g_1g_2})^{-1} \tag{10}
$$

$$
=\iota (a_{g_1})\iota (^{g_1}a_{g_2})\iota (c_{\sigma}(g_1, g_2))\iota (a_{g_1g_2})^{-1}
$$

由于群 F 是可交换的，所以我们有关系

$$
c_{\sigma'}(g_1, g_2)c_{\sigma}(g_1, g_2)^{-1}= (^{g_1}a_{g_2})a^{-1}_{g_1g_2}a_{g_1}= (\partial a)(g_1, g_2) \tag{11}
$$

由(8)得出如下。这就证明了$H^2(G,F)$重合中$c_{\sigma'}$和$c_{\sigma}$的类。

最后，令$\mathscr{E}= (\Gamma , \iota , \pi )$和$\mathscr{E}'= (\Gamma ', \iota ', \pi ')$同构的$\tau$扩展，令$u:\mathscr{E}\rightarrow \mathscr{E}'$为$\tau$扩展的态射，并令$\sigma$为映射$\pi$的截面。 映射$u\circ \sigma$是映射$\pi '$中的截面，我们有$c_{\sigma}=c_{u\circ\sigma}$。因此，$H^2(G,F)$中$c_{\sigma}$的类仅取决于Ex$_{\tau}(G,F)$中$\mathscr{E}$的类。

我们用 $\Theta_{\tau}$ 表示：Ex$_{\tau}(G,F)\rightarrow H^2(G,F)$，或更简单地 θ，映射将 $\tau$ 扩展 $(\Gamma , \iota , \pi )$ 的类发送到 2-cocycle $c_{\sigma}$ 的类，其中 $\sigma$ 是截面投影$\pi$。

#### 定理 1 {#alg-viii-s16-thm-1 .statement tag=00IR}

从 Ex$_{\tau}(G,F)$ 到 $H^2(G,F)$，映射 θ 为群同构。

我们首先证明 θ 是群同态。 令$\mathscr{E}= (\Gamma , \iota , \pi )$和$\mathscr{E}'= (\Gamma ', \iota ', \pi ')$为$\tau$扩展，并令$\sigma$（分别为$\sigma '$）为映射$\pi$（分别为$\pi '$）的截面。 我们用$\tau$扩展$\mathscr{E}$和$\mathscr{E}'$的$\mathscr{E} \mathscr{E}'= (\Gamma '', \iota '', \pi '')$乘积来表示。 我们用$[\gamma , \gamma ']$表示$\Gamma \times_G\Gamma '$的元素$(\gamma , \gamma ')$在$\Gamma ''$中的图像，通过VIII，p. 293的注解的满射同态。 从G到$\Gamma ''$的映射发送元素$g$到$[\sigma (g), \sigma '(g)]$是映射$\pi ''$的截面$\sigma ''$。 令$g_1$和$g_2$为G的元素。 我们有关系

$$
\iota ''(c_{\sigma''}(g_1, g_2)) =\sigma ''(g_1)\sigma ''(g_2)\sigma ''(g_1g_2)^{-1}
$$

$$
= [\iota (c_{\sigma}(g_1, g_2)), \iota '(c_{\sigma'}(g_1, g_2)]
$$

$$
=\iota ''(c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2))
$$

因此我们有$c_{\sigma''}(g_1, g_2) =c_{\sigma}(g_1, g_2)c_{\sigma'}(g_1, g_2)$。

让我们证明映射 θ 是单射的。令$\mathscr{E}= (\Gamma , \iota , \pi )$为$\tau$扩展，并令$\sigma$为映射$\pi$的截面，这样$H^2(G,F)$中$c_{\sigma}$的像是微不足道的。存在映射 $a: G\rightarrow F$ 使得

$$
c_{\sigma}(g_1, g_2) = (^{g_1}a(g_2))a(g_1g_2)^{-1}a(g_1)
$$

对于所有$g_1, g_2\in G$。然后我们定义 $\sigma ': G\rightarrow \Gamma$

$$
\sigma '(g) =\iota (a(g)^{-1})\sigma (g)
$$

对于$g\in G$。利用(11)，我们得到$c_{\sigma'}$是常数，值为1；因而，$\sigma '$是群同态，这证明$\tau$扩展$\mathscr{E}$是半平凡的（I, §6, No. 1，p. 67，命题4）。

让我们证明映射 θ 是满射。设$c$为$Z^2(G,F)$的元素。我们赋予集合 $\Gamma  = F\times G$ 律或合成： (12) $(f_1, g_1)(f_2, g_2) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)$

对于所有 $f_1, f_2\in F$ 和 $g_1, g_2\in G$。我们有关系

$$
(f_1, g_1) ((f_2, g_2)(f_3, g_3)) = (f_1, g_1)(f_2(^{g_2}f_3)c(g_2, g_3), g_2g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)(^{g_1}c(g_2, g_3))c(g_1, g_2g_3), g_1g_2g_3)
$$

和

$$
((f_1, g_1)(f_2, g_2)) (f_3, g_3) =(f_1(^{g_1}f_2)c(g_1, g_2), g_1g_2)(f_3, g_3)
$$

$$
=(f_1(^{g_1}f_2)(^{g_1g_2}f_3)c(g_1, g_2)c(g_1g_2, g_3), g_1g_2g_3)
$$

对于所有 $f_1, f_2, f_3\in F$ 和 $g_1,g_2, g_3\in G$。由此可见，律是结合律，因为 $c$ 是 2-余循环。对于每个 $(f, g)\in \Gamma$，我们有

$$
(f, g)(c(e, e)^{-1}, e) = (f(^gc(e, e)^{-1})c(g, e), g)
$$

现在，从 2-cocycle 的定义可以得出 $c(g, e) =^gc(e, e)$，从中我们可以推导出 $(f, g)(c(e, e)^{-1}, e) = (f, g)$。我们同样证明

$$
(c(e, e)^{-1}, e)(f, g) = (f c(e, e)^{-1}c(e, g), g) = (f, g)
$$

因而，由 (12) 定义的合成的律有单位元素 $(c(e, e)^{-1}, e)$，并且 Γ 的每个元素 $(f, g)$ 都是可逆的，有逆

$$
(^{g^{-1}}(f^{-1}c(e, e)^{-1}c(g, g^{-1})^{-1}), g^{-1})
$$

所以我们赋予 Γ 群结构。让我们用$\iota : F\rightarrow G$映射表示将$f$发送到$(c(e, e)^{-1}f, e)$，用$\pi : \Gamma \rightarrow G$表示第二个投影，并用$\sigma$映射$g\mapsto (1, g)$表示。 映射$\iota$和$\pi$是群同态，所以三元组$\mathscr{E}= (\Gamma , \iota , \pi )$是$\tau$扩展，$\sigma$是映射$\pi$的截面，以及相关的循环$c_{\sigma}$ 等于 $c$ 因为

$$
\sigma (g_1)\sigma (g_2)\sigma (g_1g_2)^{-1}= (1, g_1)(1, g_2)(1, g_1g_2)^{-1}= (c(g_1, g_2), g_1g_2)(1, g_1g_2)^{-1}
$$

$$
= (c(g_1, g_2)c(e, g_1g_2)^{-1}, e) = (c(e, e)^{-1}c(g_1, g_2), e)
$$

$g_1, g_2\in G$。

#### 注 {#alg-viii-s16-n5-rem-1 .statement tag=00RK}

设G为群，设F和$F'$为阿贝尔的群，设$\tau$（分别为$\tau '$）为从G到F的自同构群（分别为$F'$）的群同态，并令$v: F\rightarrow F'$ 为群态射使得

$$
v(\tau (g)\cdot f) =\tau '(g)\cdot v(f) \tag{13}
$$

对于 $g\in G$ 和 $f\in F$。设$\alpha$为Ex$_{\tau}(G,F)$的元素。如果余循环$c$代表$\Theta (\alpha )$，则$v\circ c$代表$\Theta (v_*(\alpha ))\in H^2(G,F')$。

### 6. 限制与余限制

令G和$G'$为群，F为阿贝尔的群，$\tau$为从G到F的自同构群的同态。令$u: G'\rightarrow G$为群同态。我们写$\tau '=\tau \circ u$。

如果$\psi : G\times G\rightarrow F$是G的2-余循环，值在F中，则$(g_1, g_2)\mapsto \psi (u(g_1), u(g_2))$给出的从$G'\times G'$到F的映射$\psi \circ (u\times u)$是$G'$的2-余循环，值在F中，并且映射$\psi \mapsto \psi \circ (u\times u)$从$Z^2(G,F)$到$Z^2(G',F)$诱导群同态$u^*: H^2(G,F)\rightarrow H^2(G',F)$。对于任意 $\lambda \in H^2(G,F)$，元素 $u^*(\lambda )$ 被 $u$ 称为 $\lambda$ 的逆像。当$G'$是G的子群且$u: G'\rightarrow G$是典范嵌入时，从G到$G'$，同态$u^*$称为限制同态；我们用 Res$^G_{G'}$ 表示它。当G为$G'$的商且$u: G'\rightarrow G$为典范满射时，从G到$G'$称为同态$u^*$为膨胀同态。

#### 命题 7 {#alg-viii-s16-prop-7 .statement tag=00IS}

在上面的记号中，以下图表通勤：

例$_{\tau}(G,F)^{u^*}$ // 例$_{\tau}(G',F)$

$\Theta_{\tau}\Theta_{\tau'}$

$H_2(G,F)^{u^*}$ // $H_2(G',F)$。

令 H 为有限指标的 G 的子群。令$s$为从G到$H\backslash G$的典范满射中的截面。我们用乘法来表示由 G 的右作用在 $H\backslash G$ 上引起的 G 的 $(g, x)\mapsto x\cdot g$ 右作用。请注意，对于每个 $x\in H\backslash G$ 和 $g\in G$，元素 $s(x)gs(x\cdot g)^{-1}$ 属于到 H。对于任何映射 $c: H\times H\rightarrow F$，我们因此可以定义映射 $\widetilde{c}_s: G\times G\rightarrow F$ 关系

$$
\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})
$$

$g_1,g_2\in G$。从$F^{H\times H}$到$F^{G\times G}$，映射$c\mapsto \widetilde{c}_s$是群同态。

#### 引理 4 {#alg-viii-s16-lem-4 .statement tag=00IT}

如果$c: H\times H\rightarrow F$是H的2-共环，值在F中，则$\widetilde{c}_s$是G的2-共环，值在F中。

令$g_1,g_2$和$g_3$为G的元素。对于每个$i\in  \{1,2,3\}$，我们通过关系定义映射$h_i: H\backslash G\rightarrow H$

$$
h_i(x) =s(x\cdot g_1\cdots g_{i-1})g_is(x\cdot g_1\cdots g_i)^{-1}
$$

$x\in H\backslash G$。请注意

$$
h_1(x)h_2(x) =s(x)g_1g_2s(x\cdot g_1g_2)^{-1}
$$

$$
h_2(x)h_3(x) =s(x\cdot g_1)g_2g_3s(x\cdot g_1g_2g_3)^{-1}
$$

$x\in H\backslash G$。那么我们就有关系

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

其中第二个等式由 $c$ 是 2-cocycle 得出。

#### 引理 5 {#alg-viii-s16-lem-5 .statement tag=00IU}

如果$c$是2-共边界，那么$\widetilde{c}_s$也是2-共边界。

令$t: H\rightarrow F$为映射，使得$c=\partial t$。令 $\widetilde{t}_s: G\rightarrow F$ 为映射定义为

$$
\widetilde{t}_s(g) =\prod_{x\in H\backslash G}^{s(x)^{-1}}t(s(x)gs(x\cdot g)^{-1})
$$

$g\in G$。只需证明$\widetilde{c}_s=\partial \widetilde{t}_s$，由关系$\widetilde{c}_s(g_1, g_2) =\prod_{x\in H\backslash G}^{s(x)^{-1}s(x)g_1s(x\cdot g_1)^{-1}}t(s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$推出

$$
\times \prod_{x\in H\backslash G}^{s(x)^{-1}}(t(s(x)g_1g_2s(x\cdot g_1g_2)^{-1})^{-1}t(s(x)g_1s(x\cdot g_1)^{-1}))
$$

$$
=\partial \widetilde{t}_s(g_1, g_2)
$$

$g_1, g_2\in G$。

#### 引理 6 {#alg-viii-s16-lem-6 .statement tag=00IV}

令 $c$ 为 H 的 2-余循环，值在 F 中。群 $H^2(G,F)$ 中$\widetilde{c}_s$ 的像不依赖于截面 $s$ 的选择。

令$s'$为从G到$H\backslash G$的典范满射中的截面。令 $h: H\backslash G\rightarrow H$ 为映射，其特征为关系

$$
s'(x) =h(x)s(x)
$$

$x\in H\backslash G$。 2-cocycle $\widetilde{c}_{s'}$ 则由关系给出

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

$\times \prod_{x\in H\backslash G}c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$$\times \prod_{x\in H\backslash G}^{g_1s(x)^{-1}}c(h(x)^{-1}, h(x)s(x)g_2s'(x\cdot g_2)^{-1})$

$s(x)^{-1}(-1''-1-1$

$$
\times \prod_{x\in H\backslash G}c(h(x), s(x)g_1g_2s(x\cdot g_1g_2))
$$

$$
\times c(h(x)^{-1}, s'(x)g_1s'(x\cdot g_1)^{-1}))
$$

对于所有$g_1, g_2\in G$。第一个等式来自余循环关系（VIII，p. 295，公式（7））应用于元素

$h(x)^{-1},h(x)s(x)g_1s'(x\cdot g_1)^{-1}$和$s'(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$；

第二个是通过应用余循环关系到元素获得

$s(x)g_1s(x\cdot g_1)^{-1},h(x\cdot g_1)^{-1}$、$h(x\cdot g_1)s(x\cdot g_1)g_2s'(x\cdot g_1g_2)^{-1}$；最后一个简单地使用了映射$x\mapsto x\cdot g_1$是$H\backslash G$的置换这一事实。

获得的表达式对应的最后两行为 2-coboundary。我们发现$\widetilde{c}_{s'}$在$H^2(G,F)$中具有与$(g_1, g_2)\in G^2$中的值由表达式给出的余循环相同的类

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

$\times c(s(x)g_1s(x\cdot g_1), h(x\cdot g_1))$$=\prod_{x\in H\backslash G}^{s(x)^{-1}}c(s(x)g_1s(x\cdot g_1)^{-1}, s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1})$

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

其中第一个等式源自应用于元素的余循环关系

$s(x)g_1s(x\cdot g_1)^{-1},s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$和$h(x\cdot g_1g_2)^{-1}$。

获得的表达式对应的最后两行为 2-coboundary。我们发现$\widetilde{c}_{s'}$重合与$\widetilde{c}_s$的类。

我们构造了从群$H^2(H,F)$到群$H^2(G,F)$的同态，我们将其称为从H到G的上限制同态，并用Cor$^G_H$表示。

#### 命题 8 {#alg-viii-s16-prop-8 .statement tag=00IW}

令 H 为有限指标的 G 的子群。 自同态 Cor$^G_H\circ$ Res$^G_H$ 群 $H^2(G,F)$ 重合与乘法 by 指标 (G : H)。

令$\alpha$为$H^2(G,F)$的元素，并令$c$为表示$\alpha$的$Z^2(G,F)$的元素。 元素 Cor$^G_H\circ$ Res$^G_H(\alpha )$ 是余循环的类，其 $(g_1, g_2)\in G^2$ 中的值由表达式给出

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

第一个等式来自余循环关系（VIII，p. 295，公式（7））应用于元素

$s(x)^{-1},s(x)g_1s(x\cdot g_1)^{-1}$、$s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$；

第二个由应用余循环关系到元素获得

$g_1,s(x\cdot g_1)^{-1}$和$s(x\cdot g_1)g_2s(x\cdot g_1g_2)^{-1}$。

通过删除余边缘，我们得到Cor$^G_H\circ$ Res$^G_H(\alpha )$是余循环的类，其$(g_1, g_2)\in G^2$中的值由表达式给出

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

这证明了结果。

### 7. 伽罗瓦代数

令 K 为交换域。如果E是K-代数，那么我们用Aut$_K(E)$表示它的自同构群。如果 E 是域 K 的伽罗瓦扩张，则群 Aut$_K(E)$ 只是伽罗瓦群 Gal(E$/K$) (V, §10, No. 2，p. 58)。

令 G 为群。 $A (K,G)$-代数是 K-代数 E 赋予群同态 $\lambda : G\rightarrow$ Aut$_K(E)$。 同态 $\lambda$ 然后赋予 E 群的结构以及 G 中的运算符，以及左 K[G] 模块的结构外法则给出：

$$
((\sum_{g\in G}\mu_gg)x=\sum_{g\in G}\mu_g\lambda (g).x \tag{14}
$$

对于 K[G] 的每 $x\in L$ 和每元素 $(\mu_g)_{g\in G}$。 $(K,G)$代数的态射是代数的态射，这也是带有运算符的群的态射。

对于$(K$, G)-代数的每个族$(E_i)_{i\in I}$，赋予其带有运算符的乘积群结构乘积 K-代数 $\prod_{i\in I}E_i$ 是一个$(K$, G)-代数。

如果E是$(K$，G)-代数，则G下E不变量的元素的集合$E^G$是E的子代数。

令 E 为 $(K$, G)-代数，其中 G 通过 $\lambda : G\rightarrow$ Aut$_K(E)$ 起作用。如果$K'$是K的扩张，那么对于任何$g\in G$，令$\lambda '(g)$是$K'$代数$L_{(K')}$的自同构Id$_{K'}\otimes \lambda (g)$。然后 $\lambda ':g\mapsto \lambda '(g)$ 赋予 $L_{(K')}$ 结构 $(K'$, G)-代数。

给定群 H和H-集合X和Y，我们用从X到Y的H-集合态射的$\mathscr{F}_H(X,Y)$集合表示。它是映射$f: X\rightarrow Y$的集合使得每 $h\in H$ 和 $x\in X$ $f(hx) =hf(x)$。

令G为群且单位元素$e$，令H为G的子群，并令E为$(K$，H)-代数。由 E 通过从 H 到 G 的共归纳法推导出来的 $(K,G)$-代数，记为 Coind$^G_H$(E)，是 K-代数 $\mathscr{F}_H(G,E)$，赋予 G 的作用，由同态 $\lambda$ 从 G 给出Aut$_K$(Coind$^G_H(E)$) 定义为

$$
(\lambda (g)\cdot f)(g') =f(g'g) \tag{15}
$$

对于$f\in$硬币$^G_H(E)$和$g, g'\in G$。

#### 引理 7 {#alg-viii-s16-lem-7 .statement tag=00IX}

a) 令 S 为 G 的子集，使得 G 的每个元素都可以唯一地写为 $hs$，其中包含 $h\in H$ 和 $s\in S$。那么将$f$发送到$(f(s))_{s\in S}$的映射就是从S到E的映射的K-代数硬币$^G_H(E)$到K-代数$\mathscr{F}(S,E)$的同构。

b) 代数 Coind$^G_H(E)$ 在 K 上有有限次数当且仅当 E 在 K 上有有限次数并且 G 中的 H 的指标是有限的。在这种情况下，我们有公式

[硬币$^G_H(E) : K] = (G : H)[E : K]$。

c) 设$E^H$为E中群H的不变量的代数，Coind$^G_H(E)^G$为Coind$^G_H(E)$中群G的不变量。 映射$f\mapsto f(e)$从Coind$^G_H(E)$到E限制到代数同构从Coind$^G_H(E)^G$到$E^H$。

断言 a) 由定义推出并隐含 b)。由(15)可知，从G到E的映射是G下Coind$^G_H(E)$不变量的元素当且仅当它与H下E不变量的值元素恒定。

#### 注 1 {#alg-viii-s16-n7-rem-1 .statement tag=00IY}

设 G 为 G 的群，G 的 H 子群，H 的 N 子群。设 E 为$(K$，N)-代数。设$\alpha$为$\mathscr{F}_H(G,\mathscr{F}_N(H,E))$中的元素。我们有关系

$$
\alpha (g)(nh) =n(\alpha (g)(h)) \tag{16}
$$

对于每个 $g\in G,h\in H$、$n\in N$ 和关系

$$
\alpha (hg)(h') = (h\alpha (g))(h') =\alpha (g)(h'h) \tag{17}
$$

对于所有$h, h'\in H$和每个$g\in G$。因而，对于每个$g\in G$和$n\in N$都有$\alpha (ng)(e) =\alpha (g)(n) =$$n(\alpha (g)(e))$。因此我们可以考虑映射

$$
\psi :\mathscr{F}_H(G,\mathscr{F}_N(H,E))\rightarrow \mathscr{F}_N(G,E)
$$

由$\mathscr{F}_H(G,\mathscr{F}_N(H,E))$中的$\alpha$和G中的$g$定义为关系$\psi (\alpha )(g) =\alpha (g)(e)$。映射$\psi$是从Coind$^G_H$（Coind$^H_N(E)$）到Coind$^G_N(E)$的代数同构，其逆发送元素$\beta$从$\mathscr{F}_N(G,E)$到映射$\alpha$由关系$\alpha (g)(h) =\beta (hg)$定义为$g\in G$和$h\in H$。

我们现在假设给定有限群 G 和有限次数的缩减 (V, §6, No. 6, p. 32) 交换K-代数 L，并赋予由同态 $\lambda$ 从 G 到 Aut$_K(L)$ 给出的 G 作用。 对于$x\in L$和$g\in G$，我们用L的自同构$\lambda (g)$下的$x$的$g\cdot x$变换来表示。 令$\mathscr{S}$为L最大理想的集合；我们用L的自同构$\lambda (g)$下的元素$\mathfrak{m}$、$\mathscr{S}$$g\cdot \mathfrak{m}$变换来表示。 是$\mathscr{S}$中的元素。 对于$\mathscr{S}$中的每个$\mathfrak{m}$，域$L/\mathfrak{m}$是K的有限扩张。 我们将投影写为$\pi_{\mathfrak{m}}: L\rightarrow L/\mathfrak{m}$，并用G中的$\mathfrak{m}$的$G_{\mathfrak{m}}$稳定子表示，即$g\in G$的集合使得$g\cdot \mathfrak{m}=\mathfrak{m}$。 K-代数$L/\mathfrak{m}$被赋予$G_{\mathfrak{m}}$的作用到同态$\lambda_{\mathfrak{m}}$，从$G_{\mathfrak{m}}$到Aut$_K(L/\mathfrak{m})$，发送$G_{\mathfrak{m}}$的元素$h$到自同构当经过到商时，$L/\mathfrak{m}$由$\lambda (h)$推出。

令$\mathscr{O}$为$\mathscr{S}$中G的轨道的集合。给定轨道 $\sigma \in \mathscr{O}$、集合 $\mathfrak{a}_{\sigma}=\bigcap_{\mathfrak{m}\in\sigma}\mathfrak{m}$ 和 $L_{\sigma}= L/\mathfrak{a}_{\sigma}$。由于$\mathfrak{a}_{\sigma}$在G下是不变的，通过经过到商，G的作用在L定义同态$\lambda_{\sigma}$从G到Aut$_K(L_{\sigma})$。最后，从L到$L_{\sigma}$用$\pi_{\sigma}$典范映射表示。

#### 引理 8 {#alg-viii-s16-lem-8 .statement tag=00RL}

a) 对于每个$g\in G,\sigma \in \mathscr{O}$和$\mathfrak{m}\in \sigma$，我们有

$[L_{\sigma}: K] =$卡片($\sigma$)$[L/\mathfrak{m}: K]$。

b) 映射 $\pi :x\mapsto (\pi_{\sigma}(x))_{\sigma\in\mathscr{O}}$ 是从 L 到 $\prod_{\sigma\in\mathscr{O}}L_{\sigma}$ 的 $(K,G)$-代数的同构。

c) 分别用$L^G($表示。 元素的L（或$L_{\sigma}$）的$L^G_{\sigma})$ 子代数在G 的作用下不变。 然后从$L^G$到$\prod_{\sigma\in\mathscr{O}}L^G_{\sigma}$$\pi$诱导同构。

由于代数 L 被减少，有限次数的交 L 的最大理想被减少到 0 (VIII, p. 173, 推论 2)。 此外，如果$\mathfrak{m}$和$\mathfrak{m}'$是L的两个不同的极大理想，那么我们有$\mathfrak{m}+\mathfrak{m}'= L$。 从 L 到 $\prod_{\mathfrak{m}\in\mathscr{S}}L/\mathfrak{m}$ 的 I, §8, No. 11、p. 110、典范映射中的命题 10 是同构，对于每$\sigma \in \mathscr{O}$，从 $L/\mathfrak{a}_{\sigma}$ 到 $\prod_{\mathfrak{m}\in\sigma}L/\mathfrak{m}$ 典范映射也是同构。 断言a)如下。 由于$\mathscr{O}$是$\mathscr{S}$的划分，因此断言b)如下； 断言 c) 是 b) 的直接的推论。

现在让我们修复 $\sigma$ 的轨道 $\sigma \in \mathscr{O}$ 和元素 $\mathfrak{m}$。 集合$F_{\mathfrak{m}}$ = Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$，并用$F_{\mathfrak{m}}$上的G的$\lambda_{F_{\mathfrak{m}}}$作用表示。对于任何$x\in L$，用从G到$L/\mathfrak{m}$的$\overline{x}$映射表示，将$g$发送到$\pi_{\mathfrak{m}}(gx)$。 [0100] 由$L/\mathfrak{m}$上VIII、p. 305公式、$G_{\mathfrak{m}}$作用定义，$\overline{x}$属于到$F_{\mathfrak{m}}$为直接的，并且从L到$F_{\mathfrak{m}}$的映射$u:x\mapsto \overline{x}$满足$g\in G$的$\lambda_{F_{\mathfrak{m}}}(g)\circ u=u\circ \lambda (g)$。在其他字中，$u$是$(K$，G)-代数的态射。

#### 引理 9 {#alg-viii-s16-lem-9 .statement tag=00IZ}

态射 $u$ 与核 $\mathfrak{a}_{\sigma}$ 是满射。 从$u$通过经过到商推出映射是从$L_{\sigma}$到$F_{\mathfrak{m}}$的$(K,G)$代数的同构。

由于$\pi_{\mathfrak{m}}$的核等于$\mathfrak{m}$，因此$u$的核等于$\bigcap_{g\in G}g^{-1}.\mathfrak{m}=\mathfrak{a}_{\sigma}$。 要证明$u$是满射，只需证明向量空间$L_{\sigma}=$$L/\mathfrak{a}_{\sigma}$和$F_{\mathfrak{m}}$在K上具有相同的维数即可。 现在，所有理想 $g\cdot \mathfrak{m}$ 在 L 中具有相同的余维，并且通过引理 8，a)，

$[L_{\sigma}: K] =$卡片($\sigma$)$.[L/\mathfrak{m}: K]$。

此外，到引理 7, b)，我们有

$$
[F_{\mathfrak{m}}: K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]
$$

由于我们有 Card($\sigma$ ) $= (G : G_{\mathfrak{m}})$，我们已经证明了等式 $[L_{\sigma}: K] =$ $[F_{\mathfrak{m}}: K]$。

此外，我们现在假设从 G 到 Aut$_K(L)$ 同态 $\lambda$ 是单射的。我们认同 K 及其像在 L 到映射 $\xi \mapsto \xi \cdot 1$。令 Ω 为 K 的代数闭扩张。从 G 到 Ω 重合的映射集合 $\mathscr{F}(G,\Omega )$，以及共生 $(\Omega$，G)-代数 Coind$^G_{\{e\}}(\Omega )$。它是秩 1 的自由 Ω[G]-模。令 $\mathscr{H}$ 为 K-代数同态从 L 到 Ω 的集合。我们在 $\mathscr{H}$ $(g, \chi )\mapsto \chi \circ \lambda (g)$ 定义右作用 。然后，Ω-代数 $\mathscr{F}(\mathscr{H},\Omega )$ 被赋予从 $\mathscr{H}$ 上 G 的右作用推导出的 $(\Omega$, G)-代数的结构。

#### 引理 10 {#alg-viii-s16-lem-10 .statement tag=00J0}

令 L 为 $(K,G)$-代数，其在 K 上的 étale。 映射 $\psi$ 从 $L_{(\Omega )}$ 到 $\mathscr{F}(\mathscr{H},\Omega )$，其特征在于关系

$$
\psi (\xi \otimes x) = (\xi \chi (x))_{\chi\in\mathscr{H}}
$$

是$(K,G)$-代数的同构。

由于L是étale，映射$\psi$是Ω代数的同构（V, §6, No. 3，p. 30，命题2和V, §6, No. 3，p. 29，命题1，c））。我们有关系

$\psi$((Id $\otimes \lambda (g)$)$(\xi \otimes x)$) $= (\xi (\chi \circ \lambda (g))(x))_{\chi\in\mathscr{H}}$

对于$\xi \in \Omega ,x\in L$和$g\in G$。所以 $\psi$ 是 $(\Omega$, G)-代数的态射。

#### 定理 2 {#alg-viii-s16-thm-2 .statement tag=00J1}

设G为有限群，并令L为有限次数的交换K-代数，赋予G的作用，由单同态$\lambda$从G到Aut$_K(L)$给出。那么以下属性是等效的：

(i) 从 H 到 Gal(E$/K$)，存在 G 的子群 H，有限次数、K 的伽罗瓦扩张 E，同构，以及从 L 到 Coind$^G_H(E)$ 的$(K,G)$-代数同构。

(ii) 代数 L 是étale，$\mathscr{H}$ 是齐次主G 集（I, §5, No. 6、p. 60、定义 7）。

(iii) 存在$(\Omega ,G)$-代数$\psi : L_{(\Omega )}\rightarrow \mathscr{F}(G,\Omega )$的同构；在其他字中，对于每个$g\in G$，$\Omega^G$的自同构$\psi \circ \lambda (g)_{(\Omega )}\circ \psi^{-1}$等于自同构

$$
(x_h)_{h\in G}\longmapsto (x_{hg})_{h\in G}
$$

(iv) 代数L减少，L是秩1的自由K[G]模。

(v) 代数 L 约简，我们有 Card(G) = [L : K]，并且 K 是 G 的作用下元素 L 不变的子环。

(vi) 减少代数 L，群 G 传递作用于 L 最大理想集合，并且对于 G 中L 的每个最大理想 $\mathfrak{m}$，$\mathfrak{m}$ 稳定子 $G_{\mathfrak{m}}$忠实地作用于 $L/\mathfrak{m}$ 并承认 K 作为不变量的子域。

(i)$\Rightarrow$(ii)：设E为从H到Aut$_K(E)$的有限次数和$\tau$同构的K的伽罗瓦扩张。令 S 为 G 模 H 的右陪集的代表系统。 K-代数 F = Coind$^G_H(E)$ 同构于 $\mathscr{F}(S,E)$ (引理 7, a))；因此它是étale。我们用F上的G的$\lambda_F$作用表示。此外，从E到Ω，令$\psi$为K-代数同态，并令从F到Ω$\chi_0$为同态$f\mapsto \psi (f(e))$。令 $g\in G$ 使得我们有 $\chi_0\circ \lambda_F(g) =\chi_0$；由于$\psi$是单射的，因此对于每个$f\in F$我们都有$f(g) =f(e)$。鉴于引理 7, a)，我们有 $g\in H$，并且由公式

$$
f(h) =\tau (h)\cdot f(e) \tag{18}
$$

对于每个 $h\in H$ 都成立，只有当 $g=e$ 时才会发生这种情况。另一方面，通过引理 7, b) 和 V, §10, No. 6、p. 66 中的定理 3，我们有

[F : K] = (G : H)[E : K] = (G : H) 卡(H) = 卡(G)。

从F到Ω的K同态的集合$\mathscr{K}$有基数[F : K]，因为F是étale（V, §6, No. 5，p. 32，命题4），所以Card（$\mathscr{K}$）$=$Card（G）。由于G中$\chi_0$的稳定子等于$\{e\}$，因此$\mathscr{K}$是同质主G集。

(ii)$\Rightarrow$(iii)：假设L是étale并且$\mathscr{H}$是同质主G集。到引理 10，$(\Omega$，G)-代数$L_{(\Omega )}$和$\mathscr{F}(\mathscr{H},\Omega )$是同构的。由于 $\mathscr{H}$ 是同质主 G 集，因此 $(\Omega$, G)-代数 $\mathscr{F}(\mathscr{H},\Omega )$ 和 $\mathscr{F}(G,\Omega )$ 是同构的。

(iii)$\Rightarrow$(iv)：假设性质(iii)成立。那么$L_{(\Omega )}$是秩1除以代数Ω[G]的自由模；后者可以被规范地识别为$K[G]_{(\Omega )}$。然后我们应用定理 3 / VIII，p. 37。

蕴涵(iv)$\Rightarrow$(v)是直接的。

让我们证明蕴涵 (v)$\Rightarrow$(vi)。 代数 L 减少。通过引理 8, c)，群 G 传递作用于 L 最大理想的集合 $\mathscr{S}$。令 $\mathfrak{m}$ 为 $\mathscr{S}$ 中的元素。到引理 9，由于$\bigcap_{\mathfrak{n}\in\mathscr{S}}\mathfrak{n}=\{0\}$，代数L同构于代数Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$。 $L/\mathfrak{m}$中$G_{\mathfrak{m}}$的不变量的代数因此重合，其中K乘以引理7，c)。因此，从 $G_{\mathfrak{m}}$ 到 Gal((L$/\mathfrak{m}$)$/K$) 的同态 $\lambda_{\mathfrak{m}}$ 是满射。到引理 7，我们还有

卡(G)$= [L : K] = (G : G_{\mathfrak{m}})[L/\mathfrak{m}: K]$。所以 Card(G$_{\mathfrak{m}}$) $= [L/\mathfrak{m}: K]$ 和同态 $\lambda_{\mathfrak{m}}$ 是单射的。

仍有待证明蕴涵(vi)$\Rightarrow$(i)。令$\mathfrak{m}$为L的最大理想。到引理 9，代数 L 作为 $(K$, G)-代数同构于代数 Coind$^G_{G_{\mathfrak{m}}}(L/\mathfrak{m})$。由于$G_{\mathfrak{m}}$忠实地作用于$L/\mathfrak{m}$并承认K为子域不变量，群同态$\lambda_{\mathfrak{m}}$定义同构从$G_{\mathfrak{m}}$到Gal((L$/\mathfrak{m}$)$/K$)。

#### 注 2 {#alg-viii-s16-n7-rem-2 .statement tag=00J2}

在定理 2 中，我们可以替换假设 Ω 是代数闭的，假设 Ω 是可分离闭的。事实上，如果L是étale，那么从L到Ω的每个K-代数同态的像是K的可分扩张。

#### 注 3 {#alg-viii-s16-n7-rem-3 .statement tag=00J3}

正常的基定理 (V, §10, No. 9, p. 73, 定理 6) 是定理 2 中蕴涵 (i)$\Rightarrow$(iv) 的特例。

#### 定义 1 {#alg-viii-s16-def-1 .statement tag=00J4}

设 G 为有限群，并令 L 为有限次数的非零的交换代数，赋予 K 赋予 $(K,G)$ 代数的结构，其中 G 的作用由从 G 到群的单同态给出自动$_K(L)$。 We say that L is a Galois algebra with group G if it has the equivalent properties (i) through (vi) of Theorem 2.

#### 注 4 {#alg-viii-s16-n7-rem-4 .statement tag=00J5}

假设L是K的扩张，赋予G的作用$\lambda$。那么L在K上是伽罗瓦代数当且仅当L是K的伽罗瓦扩张并且$\lambda$是从G到伽罗瓦群的同构 L 超过 K。

#### 注 5 {#alg-viii-s16-n7-rem-5 .statement tag=00J6}

假设群 G 是阿贝尔的。如果 G 忠实且传递地作用于集合 X，则 X 的任何点的稳定子都被约化为恒等式（因为 X 的点的稳定子都相等，并且它们的交被约化为 G 的单位元素）。因而，定理 2 的属性 (i) 到 (vi) 也等价于以下内容：

(vii) 代数 L 是étale，G 忠实且传递地作用于$\mathscr{H}$。

#### 注 6 {#alg-viii-s16-n7-rem-6 .statement tag=00J7}

V, §10, No. 1、p. 75、引理 5； V, §10, No. 1、p. 76、命题12；且 VIII、p. 137、命题 3、伽罗瓦代数是可交换的且半单。

#### 例 1 {#alg-viii-s16-n7-exa-1 .statement tag=00J8}

令$n$严格为正整数，与K的特征指数素数。假设K中单位元的$n$-第根的群$\mu_n$有阶$n$。那么对于$n$的每个除子$d$，$d$的群$\mu_d$-单位元的第根有阶$d$。令$a$为K的非零元素，令L为代数$K[X]/(X^n-a)$，令$x$为L中X的类。 序列 $(1, x, . . . , x^{n-1})$ 是向量空间 L 中的基超过域 K，我们有 $x^n=a$。此外，多项式$X^n-a$与其导数$nX^{n-1}$互质，因此代数L是étale（V, §7, No. 2，p. 37，命题3）。对于 $\mu_n$、环 K[X] 定义中的每个 $\zeta$、自同构 $P(X)\mapsto P(\zeta X)$，由经过到商、自同态 $\lambda (\zeta )$ L，因为我们有$(\zeta X)^n-a= X^n-a$；是自同构。我们有

$$
\lambda (\zeta )x^i=\zeta^ix^i \tag{19}
$$

对于$0\leqslant i < n$。从$\mu_n$到Aut$_K$(L)，映射$\lambda :\zeta \mapsto \lambda (\zeta )$为单同态，L中群$\lambda (\mu_n)$的不变量环等于$K\cdot 1$。由于$\mu_n$的基数等于$n= [L : K]$，因此赋予$\lambda$的作用的代数L为伽罗瓦代数(VIII，p. 308，定理2，(v))。

令$r$是最不严格的正整数，使得$a^r$属于到$K^{*n}$；它除$n$，并且存在$K^*$的元素$b$使得$a=b^{n/r}$。那么 (V, §11, No. 8, p. 91, 注) 多项式 $X^r-b$ 是不可约的，我们有$X^n-a=\prod_{\zeta\in\mu_{n/r}}(X^r-\zeta b)$。设E为域$K[Y]/(Y^r-b)$，$y$为E中Y的类。从$\mu_{n/r}$到Gal(E$/K$)存在同构$\theta$，其特征为关系$\theta (\xi )(y) =\xi y$ （V, §11, No. 8、p. 91、例 3）。然后我们验证伽罗瓦代数 L 与 $(K, \mu_n$)-代数 Coind$^{\mu_n}_{\mu_{n/r}}(E)$ 同构的。

#### 例 2 {#alg-viii-s16-n7-exa-2 .statement tag=00J9}

现在假设域 K 具有特征 $p\not= 0$。令 $c$ 为 K 的元素。多项式 $f= X^p-X-c$ 与其导数 $f'=-1$ 互质，因此代数 $L = K[X]/(f)$ 是 étale (V, §7, No. 2, p. 37, 命题 3)。我们用$x$表示L中X的像；我们有关系$x^p=x+c$。 序列 $(1, x, . . . , x^{p-1})$ 是 L 中的基，在 K 上被视为向量空间。

令 P 为 K 素数子域的加法群；它是阶$p$的循环群，由K的单位元1生成。对于P中的每个$j$，我们有$j^p=j$（V, §1, No. 3，p. 4，公式（4）），因此$f(X +j) =f(X)$。因此存在代数L的自同构$\gamma (j)$，其特征为关系$\gamma (j)(x) =x+j$；而且，从P到Aut$_K(L)$，所得的映射$\gamma$是单同态。

设 Ω 为 K 的代数闭扩张，并令 $\xi$ 为 Ω 中多项式 $f$ 的根。我们有 $\xi^p=\xi +c$，因此

$$
X^p-X-c= (X^p-\xi^p)-(X-\xi ) = (X-\xi )^p-(X-\xi ) =\prod_{j\in P}(X-\xi -j)
$$

由 V, §12, No. 1、p. 94、公式 (1)。对于P中的每个$j$，都存在唯一代数同态$\chi_j: L\rightarrow \Omega$将$x$发送到$\xi +j$；而且，从L到Ω的每个同态都是$\chi_j$之一，我们有关系$\chi_j=\chi_0\circ \gamma (j)$。赋予$\gamma$的代数L具有VIII、p. 308中的定理2个性质(ii)，因此伽罗瓦代数超过K。

为了描述L的结构，我们必须区分两种情况：

a) 我们有 $\xi \notin K$。那么多项式 $f(X)$ 在 K[X] 中是不可约的 (V, §11, No. 9, p. 93, 例 3)。在这种情况下，L是次数$p$的K的循环扩张，$\gamma$是从P到Gal（L$/K$）的同构。

b) 我们有 $\xi \in K$。那么映射$\psi :y\mapsto (\chi_j(y))_{j\in P}$就是同构，从代数L到乘积代数$K^P$；此外，对于每个$k\in P$，$\psi \circ \gamma (k)\circ \psi^{-1}$是$K^P$中的自同构$(x_j)_{j\in P}\mapsto (x_{j+k})_{j\in P}$。

### 8. 作用于伽罗瓦代数

#### 命题 9 {#alg-viii-s16-prop-9 .statement tag=00JA}

设G为有限群，H为G的子群，E为域K上的伽罗瓦代数和群H。则通过从H到G的共归纳，从E推导出$(K,G)$-代数Coind$^G_H(E)$为伽罗瓦代数域 K 与群 G。

由于 E 在 K 上伽罗瓦代数，通过 VIII、p. 308 的定理 2 的性质 (v) 进行约减，我们有 Card(H) = [E : K]，并且 K 是 E 中 H 的不变量的环。但是通过引理 VIII、p. 305、代数 F = Coind$^G_H(E)$ 的 7 被减少，我们有

[F : K] = (G : H)[E : K] = (G : H) 卡(H) = 卡(G)，

K 是 F 中 G 的不变量的环。因此，根据定理 2, (v) 中给出的标准，F 是伽罗瓦代数。

#### 命题 10 {#alg-viii-s16-prop-10 .statement tag=00JB}

设G为有限群。令 L 为域 K 上的群 G 上的伽罗瓦代数，并令 $K'$ 为 K 上的扩张。则 $(K',G)$ 代数 $L_{(K')}$ 为 $K'$ 上的伽罗瓦代数。

我们通过注意到在定理2中使用性质(v)，如果K-代数L是étale，那么$K'$-代数$L_{(K')}$也是(V, §6, No. 5，p. 32，推论2)，我们有等式$[L_{(K')}: K'] = [L : K]$，并且$L_{(K')}$中G的不变量环是$(L^G)_{(K')}$，其中$L^G$是L中G的不变量环。

#### 命题 11 {#alg-viii-s16-prop-11 .statement tag=00JC}

令$G_1$和$G_2$为群。令$L_1$和$L_2$在K上为伽罗瓦代数，分别为作用$\lambda_1: G_1\rightarrow$Aut$_K(L_1)$和$\lambda_2: G_2\rightarrow$Aut$_K(L_2)$。 集合 $L = L_1\otimes_KL_2,G = G_1\times G_2$，$\lambda (g_1, g_2) =\lambda_1(g_1)\otimes \lambda_2(g_2)$ $(g_1, g_2)\in G$。那么K-代数L赋予作用$\lambda$就是伽罗瓦代数超过K。

我们将其推理为之前，并考虑以下因素：如果 $L_1$ 和 $L_2$ 是 étale，那么代数 $L = L_1\otimes_KL_2$ 也是 étale（V, §6, No. 5、p. 32、推论 1），并且我们有等式

$[L : K] = [L_1: K][L_2: K]$ 和卡(G) = 卡(G$_1$) 卡(G$_2$)。

此外，如果$L^{G_i}_i$表示$L_i$中$G_i$的不变量的环，则从下面的引理11可以得出，$L^{G_1}_1\otimes_KL^{G_2}_2$是$L_1\otimes_KL_2$中$G_1\times G_2$的不变量的环。

#### 引理 11 {#alg-viii-s16-lem-11 .statement tag=00JD}

令$G_1$和$G_2$为群，令$W_1$和$W_2$为K-向量空间。我们分别捐赠$W_1($。 $W_2)$ 与作用或 $G_1($。 $G_2)$ 由群同态 $\rho_1: G_1\rightarrow$ Aut$_K(W_1) ($resp 给出。 $\rho_2: G_2\rightarrow$自动$_K(W_2))$。我们考虑群同态

$\rho_1\otimes \rho_2: G_1\times G_2\longrightarrow$ 自动$_K(W_1\otimes_KW_2)$

对于$g_1\in G_1,g_2\in G_2,w_1\in W_1$和$w_2\in W_2$，由关系$(\rho_1\otimes \rho_2)(g_1, g_2)(w_1\otimes w_2) =\rho_1(g_1)(w_1)\otimes \rho_2(g_2)(w_2)$定义。 然后，由正则注入的张量积给出的从$W^{G_1}_1\otimes_KW^{G_2}_2$到$W_1\otimes_KW_2$的线性映射导致了从$W_1^{G_1}\otimes_KW^{G_2}_2$到$(W_1\otimes_KW_2)^{G_1\times G_2}$的K向量空间的同构。

这是从应用于 K[G]-模块 $M_1= M_2= K$ 的 VIII、p. 213 的引理 1 得出的，赋予了$G, N_1= W_1$ 和$N_2= W_2$ 的平凡作用。

#### 注 {#alg-viii-s16-n8-rem-1 .statement tag=00JE}

令L为有限次数的域K的伽罗瓦扩张，并令G为其伽罗瓦群；我们用$\lambda$表示G上的恒等映射。那么L赋予$\lambda$是伽罗瓦代数超过K和群G。令$K'$是K的扩张。到命题10，代数$L_{(K')}$是伽罗瓦超过$K'$，但它不在一般扩张 $K'$。类似地，由命题11，伽罗瓦扩张E的张量积和有限次数K的F可看成伽罗瓦代数；一般来说，它不是 K 的伽罗瓦扩张。然而，如果 E 和 F 而且是 K 的扩张的线性不相交的子扩展（V, §2, No. 5、p. 13 和 V, §10, No. 1、p. 57、命题 1）。

### 9. 叉积

令K为域，令G为群，其单位元素我们用$e$表示。令L为交换K-代数，令$\lambda$为从G到K-代数L的自同构群的同态。对于G中的任何$g$，令$\tau (g)$是$\lambda (g)$诱导的L的乘法群$L^*$的自同构。

设$\mathscr{E}= (\Gamma , \iota , \pi )$是群G的$\tau$扩展$L^*$。 集合 $L\times \Gamma$ 群 $L^*$ 的定义右作用

$$
(\beta , \gamma ).\alpha = (\beta \alpha , \iota (\alpha )^{-1}\gamma ) \tag{20}
$$

对于 $\alpha \in L^*,\beta \in L$ 和 $\gamma \in \Gamma$。我们用$L\times \Gamma$中$L^*$的轨道的E集合和对$(\beta , \gamma )$的$[\beta ;\gamma ]$轨道表示。因此，到构造，我们有关系

$$
[\beta \alpha ;\gamma ] = [\beta ;\iota (\alpha )\gamma ] \tag{21}
$$

对于 $\alpha \in L^*,\beta \in L$ 和 $\gamma \in \Gamma$。

给定 L 中的 $\beta$ 和 Γ 中的 $\gamma$，我们用 L 的自同构 $\lambda \circ \pi (\gamma )$ 下的 $\beta$ 的 $^{\gamma}\beta$ 变换表示；我们有关系

(22)$^{\gamma}(^{\gamma'}\beta ) =^{\gamma \gamma'}\beta  ,^{\gamma}(\beta +\beta ') =^{\gamma}\beta +^{\gamma}\beta '$、$^{\gamma}(\beta \beta ') =^{\gamma}\beta^{\gamma}\beta '$

对于 Γ 中的 $\gamma , \gamma '$ 和 L 中的 $\beta , \beta '$。 E 上存在合成的律，其特征为关系

$$
[\beta ;\gamma ][\beta ';\gamma '] = [\beta^{\gamma}\beta ';\gamma \gamma '] \tag{23}
$$

事实上，如果我们分别将替换、$\beta ,\gamma ,\beta '$、$\gamma '$与$\beta \alpha ,\iota (\alpha )^{-1}\gamma ,\beta '\alpha '$、以及$\iota (\alpha ')^{-1}\gamma '$（对于$L^*$中的所有$\alpha ,\alpha '$）来说，就足以验证右侧不是变换。紧接着是VIII、p. 285的应用到$\mathscr{E}$公式 (1)，对于$\gamma \in \Gamma$和$\alpha \in L^*$也可以写成$\gamma \iota (\alpha ) =\iota (^{\gamma}\alpha )\gamma$。由(22)中的公式，赋予律的集合E是一个具有单位元素$[1;e]$的幺半群。

由于$\pi \circ \iota$与值$e$恒定，因此从E到G存在映射$\widetilde{\pi}$，这样我们有

$$
\widetilde{\pi}([\beta ;\gamma ]) =\pi (\gamma ) \tag{24}
$$

对于 $\beta \in L$ 和 $\gamma \in \Gamma$。

令$g$为G的元素，并令$E_g=\widetilde{\pi}^{-1}(g)$。如果$\gamma_0$是$\pi^{-1}(g)$的固定元素，那么映射$\beta \mapsto [\beta ;\gamma_0]$就是从L到$E_g$的双射，因此我们将转移到$E_g$K-向量空间结构 L。由于$\pi^{-1}(g)$是由形式$\iota (\alpha )\gamma_0$的元素组成，其中$\alpha$贯穿$L^*$，我们有

$$
[\beta ;\iota (\alpha )\gamma_0] = [\beta \alpha ;\gamma_0]
$$

$E_g$ 上的向量空间结构不依赖于$\gamma_0$ 的选择。

设$g$和$g'$为G的元素；通过公式 (22) 和 (23)，E 诱导上合成的律通过限制从 $E_g\times E_{g'}$ 到 $E_{gg'}$ 的 K 双线性映射。因而，向量空间 $P =\bigoplus_{g\in G}E_g$ 被赋予了结合和单位代数的结构，其乘法诱导是前一个双线性映射从$E_g\times E_{g'}$到$E_{gg'}$对于所有$g$和G中的$g'$。代数P称为L和$\mathscr{E}$的叉积，记为$\mathbf{A}[\mathscr{E}; L]$；它的单位元是$E_e$的元素$[1;e]$。

集合

$$
u(\beta ) = [\beta ;e] \tag{25}
$$

L 中的 $\beta$。那么$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$就是K-代数的单同态。根据(23)，对于每个$\gamma \in \Gamma$，元素$[1;\gamma ]$在$\mathbf{A}[\mathscr{E},L]$中是可逆的，并且将$\gamma$发送到$[1;\gamma ]$的映射$v: \Gamma \rightarrow \mathbf{A}[\mathscr{E},L]^*$是单射群同态。 同态 $u$ 和 $v$ 称为规范。我们有关系

$$
u(\alpha ) =v(\iota (\alpha )) \tag{26}
$$

$$
u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1} \tag{27}
$$

$$
[\beta ;\gamma ] =u(\beta )v(\gamma ) \tag{28}
$$

对于 $\alpha \in L^*,\beta \in L$ 和 $\gamma \in \Gamma$。

相反，我们有以下泛性质或代数 $\mathbf{A}[\mathscr{E}; L]$。

#### 命题 12 {#alg-viii-s16-prop-12 .statement tag=00JF}

设 B 为 K-代数、$u': L\rightarrow B$ K-代数同态、$v': \Gamma \rightarrow B^*$ 群同态。我们假设满意关系

$$
u'(\alpha ) =v'(\iota (\alpha )) \tag{29}
$$

$$
u'(^{\gamma}\beta ) =v'(\gamma )u'(\beta )v'(\gamma )^{-1} \tag{30}
$$

$\alpha \in L^*,\beta \in L$和$\gamma \in \Gamma$。那么从$\mathbf{A}[\mathscr{E}; L]$到B存在唯一代数同态$f$，这样我们就有$u'=f\circ u$和$v'=f\circ v$。

为了证明$f$的唯一性，观察域K上的向量空间$\mathbf{A}[\mathscr{E}; L]$是由形式$[\beta ;\gamma ] =u(\beta )v(\gamma )$的元素的集合生成。如果同态$f':\mathbf{A}[\mathscr{E}; L]\rightarrow B$满足$f'\circ u=u'$和$f'\circ v=v'$，则它将$[\beta ;\gamma ]$发送到$u'(\beta )v'(\gamma )$，因此将重合发送到$f$。

到公式 (29)，我们有

$$
u'(\beta \alpha )v'(\iota (\alpha )^{-1}\gamma ) =u'(\beta )v'(\gamma ) \tag{31}
$$

对于 L 中的 $L^*,\beta$ 中的 $\alpha$，以及 Γ 中的 $\gamma$。通过E的定义，因此存在映射$f_0: E\rightarrow B$，使得$f_0([\beta ;\gamma ]) =u'(\beta )v'(\gamma )$。通过公式 (23) 和 (30)，我们对 E 中的 $x$ 和 $x'$ 有 $f_0(xx') =f_0(x)f_0(x')$。对于 G 的每个元素 $g$，$f_0$ 到 $E_g$ 的限制是 K 线性的；因而，存在从$\mathbf{A}[\mathscr{E}; L]$到B的唯一的K-线性映射$f$，重合与E上的$f_0$。映射$f$是满足$u'=f\circ u$的代数态射并且$v'=f\circ v$。

#### 注 {#alg-viii-s16-n9-rem-1 .statement tag=00JG}

设$\sigma : G\rightarrow \Gamma$为映射$\pi$中的截面。 集合$\varepsilon_g=v(\sigma (g))$对于G中的每个$g$，并用$c_{\sigma}$表示与$\sigma$相关的2-余循环（VIII，p. 296）。特别是，我们有

$$
\varepsilon_g\varepsilon_{g'}=u(c_{\sigma}(g, g'))\varepsilon_{gg'} \tag{32}
$$

对于所有$g, g'\in G$。此外，让我们通过同态$u$将认同L与子代数进行$\mathbf{A}[\mathscr{E}; L]$。那么$\mathbf{A}[\mathscr{E}; L]$的每个元素都可以唯一地写成$\sum_{g\in G}a_g\varepsilon_g$，其中$(a_g)$是L的元素与有限支撑的族。 $\mathbf{A}[\mathscr{E}; L]$中的乘法可以用公式表示

$$
(\sum_ga_g\varepsilon_g)(\sum_gb_g\varepsilon_g)=\sum_gd_g\varepsilon_g \tag{33}
$$

与

$$
d_g=\sum_{hh'=g}a_h(\lambda (h)\cdot b_{h'})c_{\sigma}(h, h') \tag{34}
$$

如果扩张$\mathscr{E}$是半平凡的，那么我们可以从G到选择截面$\sigma$$\pi$，即群态射；因而，余循环 $c_{\sigma}$ 恒定为值 1，并且公式 (34) 简化为

$$
d_g=\sum_{hh'=g}a_h\lambda (h)\cdot b_{h'} \tag{35}
$$

设$K'$为域K的扩张。用$L'$表示$K'$-代数$L_{(K')}$，对于G中的任何$g$，用$\lambda '(g)$自同构$\lambda (g)_{(K')}$表示由$\lambda (g)$诱导$L_{(K')}$。此外，让我们用由$\lambda '(g)$引起的$L^{'*}$的$\tau '(g)$自同构来表示。最后，令$h$为从$L^*$到$L^{'*}$的同态，将$x$发送到$x\otimes 1$。令$\mathscr{E}'= (\Gamma ', \iota ', \pi ')$乘以$h$(VIII，p. 289)为$\mathscr{E}$扩张直接像。令$\mathbf{A}[\mathscr{E}',L']$为叉积$K'$-$\mathscr{E}'$和$L'$的代数，并令$u': L'\rightarrow \mathbf{A}[\mathscr{E}',L']$和$v': \Gamma '\rightarrow \mathbf{A}[\mathscr{E}',L']^*$为典范同态。

#### 命题 13 {#alg-viii-s16-prop-13 .statement tag=00JH}

$K'$-代数$\varphi$从$\mathbf{A}[\mathscr{E}; L]_{(K')}$到$\mathbf{A}[\mathscr{E}'; L']$存在唯一的同构满足关系

$$
u'(h(\beta )) =\varphi (1\otimes u(\beta )) \tag{36}
$$

对于 $\beta \in L$ 和

$$
v'(h(\gamma )) =\varphi (1\otimes v(\gamma )) \tag{37}
$$

$\gamma \in \Gamma$。

证明紧接在构造之后。

同构 $\varphi$ 称为规范。

### 10. 申请布劳尔群

在这个小节中，K是域，L是K上的伽罗瓦代数和作用$\lambda : G\rightarrow$Aut$_K(L)$。我们将 K 上的 L 的次数表示为 $n$。我们有$n=$卡(G)。

#### 定理 3 {#alg-viii-s16-thm-3 .statement tag=00JI}

设$\mathscr{E}= (\Gamma , \iota , \pi )$是G的$\tau$扩展$L^*$。 代数$\mathbf{A}[\mathscr{E}; L]$是中心简单且次数$n^2$超过K。此外，典范同态$u$从L到$\mathbf{A}[\mathscr{E}; L]$是同构从L到最大交换子代数 $\mathbf{A}[\mathscr{E}; L]$。

#### 引理 12 {#alg-viii-s16-lem-12 .statement tag=00JJ}

a) 除了在G下不变的$\{0\}$和L之外，不存在L的任何理想。

b) 令$g$为与单位元素不同的G的元素，并令$\mathfrak{a}_g$为由形式$x-\lambda (g)x$的元素生成的L的理想，其中$x$贯穿L。我们有$\mathfrak{a}_g= L$。

令$\mathscr{S}$为L最大理想的集合；对于 $\mathscr{S}$、集合 $\mathfrak{a}(S) =\bigcap_{\mathfrak{m}\in S}\mathfrak{m}$ 的任意子集 S。由于环 L 是可交换的且半单 (VIII, p. 310, 注 6)，映射 $W\mapsto \mathfrak{a}(W)$ 是双射从集合到子集 L（VIII、p. 142、命题 9）的理想的$\mathscr{S}$至集合。当且仅当 S 不变时，理想的 $\mathfrak{a}(S)$ 在 G 下是不变的。由于 G 传递作用于 $\mathscr{S}$ (VIII, p. 308, 定理 2, vi))，因而 G 下 $\mathscr{S}$ 中唯一不变的子集是 $\emptyset$ 和 $\mathscr{S}$。从$\mathfrak{a}(\emptyset ) = L$和$\mathfrak{a}(\mathscr{S}) =\{0\}$开始，我们已经证明了断言a)。

让我们用反证法来证明b)；假设我们有$\mathfrak{a}_g\not= L$。令$\mathfrak{m}$为L包含$\mathfrak{a}_g$的最大理想。然后，对于L中的每个$x$，我们都有$\lambda (g)x\equiv x$ mod $\mathfrak{m}$。特别是，$\mathfrak{m}$在$g$下是不变的，而$\lambda (g)$是由域$L/\mathfrak{m}$上的恒等性引发的。由VIII的定理 2、p. 308、$G_{\mathfrak{m}}$的元素$g$中的性质(vi)来说是微不足道的，其中b)的与……矛盾假设。

现在让我们证明定理 3. 向量空间 $\mathbf{A}[\mathscr{E}; L]$ 在 K 上有有限维 Card(G)[L$: K] =n^2$，通过 VIII、p. 316 和假设的等式 Card(G) $= [L : K] =n$。

令$\mathfrak{a}$为非零的代数$\mathbf{A}[\mathscr{E}; L]$的两侧理想。我们使用VIII、p. 316中的记号。 $\mathbf{A}[\mathscr{E}; L]$的每个元素$a$都可以唯一地写为$a=\sum_{g\in G}a_g\varepsilon_g$，每个$g\in G$可以写为$a_g\in L$；我们用G的元素$g$的$\Phi (a)$集合来表示$a_g\not= 0$。到 VIII、p. 316 的公式 (32) 时，我们有关系

$$
\varepsilon_g\varepsilon_{g'}=c_{\sigma}(g, g')\varepsilon_{gg'} \tag{38}
$$

对于所有 $g, g'\in G$ ，因而

$$
\Phi (a\varepsilon_g) = \Phi (a).g \tag{39}
$$

对于每个 $g\in G$ 和 $a\in \mathbf{A}[\mathscr{E}; L]$。

令$a$为$\mathfrak{a}$的非零元素，其中$\Phi (a)$对于包含而言是最小的；由公式 (39)，如果有必要替换 $a$ 与元素或形式 $a\varepsilon_{g^{-1}}$ 与 $g\in \Phi (a)$，我们可以假设我们有 $e\in \Phi (a)$。令 $s$ 为与 $e$ 不同的 $\Phi (a)$ 的元素。到引理 12，b)，存在L的元素$x$，使得$a_s(x-\lambda (s)\cdot x)\not= 0$。但我们有关系

$$
xa-ax=\sum_ga_g(x-\lambda (g)\cdot x)\varepsilon_g \tag{40}
$$

其中和取代了$\Phi (a)$的元素$g$，与$e$不同。由于 $\Phi (a)$ 极小，因此我们有 $xa-ax= 0$，但是 $x$ 上有与……矛盾假设。因而，我们通过反证法证明G的$\Phi (a)$包含只有单位元素$e$，所以我们有$a\in L$。

因而 $L\cap \mathfrak{a}$ 是 L 的理想值，未简化为 $\{0\}$。此外，对于L中的每个$x$，我们有$\varepsilon_gx\varepsilon^{-1}_g=\lambda (g)\cdot x$，因而$L\cap \mathfrak{a}$在G下是不变的。到引理12，我们因此有$L\cap \mathfrak{a}= L$，即$L\subset \mathfrak{a}$。从$\mathbf{A}[\mathscr{E}; L]$的L包含单位元素开始，我们有$\mathfrak{a}=\mathbf{A}[\mathscr{E}; L]$。

由于代数 $\mathbf{A}[\mathscr{E}; L]$ 的非零有限维超过 K，并且其唯一的两侧理想是 $\{0\}$ 和 $\mathbf{A}[\mathscr{E}; L]$，所以它很简单。

让我们证明$\mathbf{A}[\mathscr{E}; L]$的每个元素$a$都可以与L属于通勤到L。我们将$a$写为$\sum_{g\in G}a_g\varepsilon_g$，并在L中写出系数$a_g$。对于L中的每个$x$，我们有$xa-ax= 0$，并且关系（40）表明我们有

$$
a_g(x-\lambda (g)\cdot x) = 0 \tag{41}
$$

对于每个$g\in G$和$x\in L$。因而，到引理 12 时，我们就有 $a_g= 0$ 对应 $g\not=e$；因而，$a\in L$。

最后，让我们来计算$\mathbf{A}[\mathscr{E}; L]$的确定中心。如果 $z$ 属于到中心，则它与 L 通勤，因此属于到 L。但我们有

$$
0 =\varepsilon_gz-z\varepsilon_g= (\lambda (g)\cdot z-z)\varepsilon_g
$$

对于G的每个$g$。因而$z$在L的自同构群$\lambda (G)$下是不变的。因此我们有$z\in K$乘假设。

#### 定理 4 {#alg-viii-s16-thm-4 .statement tag=00JK}

设A是K上有限次数的中心单代数，并令L是A的最大交换子代数。则存在G的$\tau$扩展$\mathscr{E}$$L^*$，使得A与$\mathbf{A}[\mathscr{E}; L]$同构的。

不失一般性，我们可以假设 L 是 A 的最大值交换子代数。令 Γ 为 A 的可逆元 $\gamma$ 的乘法群由……组成，使得 G 中存在$g$，其中

$$
\gamma x\gamma^{-1}=\lambda (g).x \tag{42}
$$

对于 L 中的每元素 $x$。如果给定$\gamma \in \Gamma$，那么元素$g$满足这个关系是唯一的；我们用$\pi (\gamma )$表示。从 Γ 到 G，$\pi$ 为同态，且其核等于 $L^*$，则为直接的。 $\pi$ 的满射性源自 Skolem–Noether 定理 (VIII, p. 263, 推论)。

如果我们用 $\iota$ 来表示$L^*$ 到 Γ 的规范注入，那么从结构中可以得出$\mathscr{E}= (\Gamma , \iota , \pi )$ 是 G $L^*$ 的 $\tau$ 扩展。 让

$u: L\rightarrow \mathbf{A}[\mathscr{E}; L]$ 和 $v: \Gamma \rightarrow \mathbf{A}[\mathscr{E}; L]$

是典范同态。通过$\mathbf{A}[\mathscr{E}; L]$（VIII，p. 315，命题 12）的泛性质，存在唯一代数同态$f:\mathbf{A}[\mathscr{E}; L]\rightarrow A$，使得$f\circ u(x) =x$和$f\circ v(\gamma ) =\gamma$对于$x\in L$和$\gamma \in \Gamma$。由于代数 $\mathbf{A}[\mathscr{E}; L]$ 很简单，因此同态 $f$ 是单射的。现在，代数$\mathbf{A}[\mathscr{E}; L]$对K有次数$n^2$，A也是如此，因为L是A的最大交换半单子代数，并且我们有$n= [L : K]$（VIII，p. 262，命题3， (二))。因此 $f$ 是双射的。

#### 定义 2 {#alg-viii-s16-def-2 .statement tag=00JL}

令$\mathscr{S}$为L最大理想的集合。我们定义

Br(L$/K$) $=\bigcap_{\mathfrak{m}\in\mathscr{S}}$ Ker($r_{(L/\mathfrak{m})/K}$)，其中 $r_{(L/\mathfrak{m})/K}:$ Br(K) $\rightarrow$ Br(L$/\mathfrak{m}$) 是标量同态的扩张 （VIII，p. 281）。

#### 定理 5 {#alg-viii-s16-thm-5 .statement tag=00JM}

存在群同构

Ψ : Ex$_{\tau}(G,L^*)\longrightarrow$ Br(L$/K$)

将G的$\tau$扩展$\mathscr{E}$的类通过$L^*$发送到代数$\mathbf{A}[\mathscr{E}; L]$的Br(L$/K$)中的类。

为了定义Ψ并验证它是双射，我们必须建立以下点：

a) 如果$\mathscr{E}$和$\mathscr{E}'$同构$\tau$-G的$L^*$扩展，则代数$\mathbf{A}[\mathscr{E}; L]$和$\mathbf{A}[\mathscr{E}'; L]$同构。

b) 相反，如果代数 $\mathbf{A}[\mathscr{E}; L]$ 和 $\mathbf{A}[\mathscr{E}'; L]$ 同构，则 G 的 $L^*$ 的 $\tau$ 扩展 $\mathscr{E}$ 和 $\mathscr{E}'$ 也是同构的。

c) 在 Br(L$/K$) 中的每个类中，都有代数 E 包含 L 作为最大交换子代数。

d) 如果 E 是有限次数的中心单代数在 K 包含 L 上作为最大值交换子代数，则存在 G 的 $\tau$ $\mathscr{E}$ $L^*$ 扩展，使得 E 与 $\mathbf{A}[\mathscr{E}; L]$ 同构。

断言 a) 由构造或叉积得出； b) 由VIII、p. 263、推论得出。 断言 c) 由 VIII、p. 281 中的命题 5 得出，而 d) 只是上面的定理 4。

还需要验证 Ψ 是否为群同态；为此，只需证明如果$\mathscr{E}_1= (\Gamma_1, \iota_1, \pi_1)$和$\mathscr{E}_2= (\Gamma_2, \iota_2, \pi_2)$是$\tau$扩展，则代数$\mathbf{A}[\mathscr{E}_1\mathscr{E}_2; L]$等价于代数$\mathbf{A}[\mathscr{E}_1; L]\otimes \mathbf{A}[\mathscr{E}_2; L]$。 我们用$\mathscr{E}= (\Gamma , \iota , \pi )$表示乘积扩张$\mathscr{E}_1\mathscr{E}_2$。 群 Γ 同构于从 $L^*$ 到将 $\mu$ 发送到 $(\iota_1(\mu), \iota_2(\mu)^{-1})$ 的纤维乘积 $\Gamma_1\times_G\Gamma_2$ 的同态 $\rho$ 的焦核。 对于$i\in  \{1,2\}$，写为$A_i=\mathbf{A}[\mathscr{E}_i; L]$。 令$u_i: L\rightarrow A_i$和$v_i: \Gamma_i\rightarrow A^*_i$为典范同态。 我们将认同L及其像乘以同态$u_i$，这使得L成为$A_i$的最大值交换子代数。 我们用$V_i$表示由$A_i$中的左乘法定义的L向量空间。 环$L\otimes_KA^o_i$作用于$V_i$。 由于它很简单并且维数$n^2$超过L，因此我们从$L\otimes_KA^o_i$到End$_L(V_i)$获得同构。 因此，环$L\otimes_KA^o_1\otimes_KA^o_2$，我们将可以确定与$(L\otimes_KA^o_1)\otimes_L(L\otimes_KA^o_2)$同构的，与End$_L(V_1\otimes_LV_2)$同构的。 集合C=结束$_{A^o_1\otimes_KA^o_2}(V_1\otimes_LV_2)$。 通过VIII、p. 282、环、C的引理 3，与$A_1\otimes_KA_2$相似，$L\otimes 1\otimes 1$是C的最大交换子代数。 对于每个对 $(\gamma_1, \gamma_2)\in \Gamma_1\times \Gamma_2$ 满足 $\pi_1(\gamma_1) =\pi_2(\gamma_2)$，我们用 $w(\gamma_1, \gamma_2)$ 表示唯一的 $\lambda (\pi_1(\gamma_1$))-半线性 (II, §1, No. 13, p. 223) 自同态，使得

$$
w(\gamma_1, \gamma_2)(x_1\otimes x_2) =v_1(\gamma_1)x_1\otimes v_2(\gamma_2)x_2
$$

对于 $x_1\in V_1$ 和 $x_2\in V_2$。我们有$w(\gamma_1, \gamma_2)\in C^*$，$w$是从纤维乘积$\Gamma_1\times_G\Gamma_2$到$C^*$的群同态。这个同态对于$\rho$和诱导同态$v$从$C^*$的像来说是微不足道的。用 $u: L\rightarrow C$ 表示，态射由 $u:\ell \mapsto \ell \otimes 1\otimes 1$ 给出。我们可以验证关系

$u(\alpha ) =v(\iota (\alpha ))$ 和 $u(^{\gamma}\beta ) =v(\gamma )u(\beta )v(\gamma )^{-1}$

对于$\alpha \in L^*,\beta \in L$和$\gamma \in \Gamma$。 VIII、p. 315中的命题 12给出从代数$\mathbf{A}[\mathscr{E}; L]$到C的同态$f$。由于代数 $\mathbf{A}[\mathscr{E}; L]$ 很简单，因此同态 $f$ 是单射的。 代数 C 和 $\mathbf{A}[\mathscr{E}; L]$ 在 K 上具有相同的维数，因此 $f$ 是同构。

#### 注 1 {#alg-viii-s16-n10-rem-1 .statement tag=00JN}

如果L是K上的代数，G是L的自同构群，那么代数$\mathbf{A}[\mathscr{E}; L]$并不总是中心简单（例如，我们可以取$L = K^n$和$G =\mathfrak{S}_n$）。

#### 注 2 {#alg-viii-s16-n10-rem-2 .statement tag=00JO}

我们可以通过有限伽罗瓦扩张L和群G将计算与代数分裂的相关联的2-同环$c$如下。 首先，存在 K-同态 $\varphi : A\rightarrow \mathbf{M}_m$(L)，其中 $[A : K] =m^2$。 对于$g\in G$，令$\varphi^g$为从A到$\mathbf{M}_m(L)$的同态，由$a\mapsto \varphi (g^{-1}ag)$给出。 根据 Skolem–Noether 定理 (VIII, p. 256, 定理 3)，对于每个 $g\in G$，存在元素 $u_g$ 的 $\mathbf{G}\mathbf{L}_m(L)$ 使得

$$
\varphi^g(a) =u_g\varphi (a)u^{-1}_g
$$

对于$a\in A$。然后我们集合

$$
c(g, g') =u_gu_{g'}u^{-1}_{gg'}
$$

我们还可以使用$\varphi :$通过$L^*$来计算G的定义扩张，我们考虑$\gamma$的群$\Gamma \subset \mathbf{G}\mathbf{L}_m(L)$由……组成，其中存在$g\in G$

$$
\varphi^g(a) =\gamma \varphi (a)\gamma^{-1}
$$

对于每个$a\in A$。该扩张的类由A的类Ψ在Br(L$/K$)中为逆像。

#### 推论 {#alg-viii-s16-n10-cor-1 .statement tag=00JP}

映射$\Phi_{L/K}= \Theta \circ \Psi^{-1}$定义群同构从Br(L$/K$)到$H^2(G,L^*)$。

设 $K'$ 为 K 的扩张，且 $\varphi : K'\rightarrow L$ 态射为 K-代数。 G 的元素 $h$ 的集合 H，使得 $\lambda (h)\circ \varphi =\varphi$ 是 G 的子群，并且赋予 $\lambda$ 的限制到 H 的$K'$-代数 L 超过伽罗瓦代数 $K'$。

#### 命题 14 {#alg-viii-s16-prop-14 .statement tag=00JQ}

以下图表通勤：

Br(L$/K$)$^{\Phi_{L/K}}/$/ $H_2(G,L_*)$

$r_{K'/K}$ 资源$^G_H$

Br(L$/K'$)$^{\Phi_{L/K'}}/$/$H_2(H,L_*)$ .

这是从 VIII、p. 299 的命题 7 和VIII、p. 317 的 13 得出的。

### 11. 指数与指数

#### 定理 6 {#alg-viii-s16-thm-6 .statement tag=00JR}

设 K 为交换域，并设 A 为 K 上有限次数的中心单A-代数。设 L 为有限次数 K 的可分扩张，即代数 A 的分裂域。则 [L : K][A] 为零 Br（K）。

存在L的扩张M，即有限次数的K的伽罗瓦扩张(V, §10, No. 1，p. 57，命题2)。 K 属于到子群 Br(M$/K$) 的布劳尔群中 A 的类 [A]。令G为M在K上的伽罗瓦群，并令$\alpha$为$H^2(G,M^*)$中[A]的像（VIII，p. 321，推论）。令 H 为 M 的伽罗瓦群除以 L。那么 H 就是 G 中指标 [L : K] 的子群 (V, §10, No. 7, p. 68, 推论 5)。由于 Res$^G_H(\alpha ) = \Phi_{M/L}(A_{(L)})$ (命题 14)，我们有 Res$^G_H(\alpha ) = 0$。根据VIII、p. 303的命题 8，得出$[L : K]\alpha = 0$，因而 [L : K][A] = 0。

设 K 为交换域，并令 A 为 K 上有限次数的中心单代数。则 A 同构于形式 $\mathbf{M}_n$(D) 的代数，其中 D 为域和中心 K，且 Br(K) 中 [A] = [D]。 D 的约化次数仅取决于 A。我们称其为 A 的约化次数指标。除的指标是 A 的约化次数。A 的指数是布劳尔群中 A 的类阶 K 的。

#### 推论 1 {#alg-viii-s16-thm-6-cor-1 .statement tag=00JS}

有限次数的中央单代数的指数超过交换域除其指标。

只要证明有限次数的域 D 超过其中心 K 就足够了。令 L 为 D 的极大交换子域，即 K 的可分扩张；我们有 $[D : K] = [L : K]^2$ (VIII, p. 265, 推论 2, b) 和 c))。那么对于代数 D (VIII, p. 281, 命题 5)，K 的扩张 L 是分裂域，并且 [L : K] 重合与 D 的减少的次数。 应用定理6.

#### 推论 2 {#alg-viii-s16-thm-6-cor-2 .statement tag=00JT}

令 K 为交换域，并令 A 为 K 上有限次数的中心单代数。令 $p$ 为素数数。若 A $p$ 除指标，则 A 除指数。

假设 A 的素数数 $p$ 不除指数，并证明它不除指标。只要A为域的情况下就足以证明这个结果。令L为分裂的A的有限次数K伽罗瓦扩张。令G为K上L的伽罗瓦群，并令H为G的Sylow$p$子群(I, §6, No. 6，p. 78)。我们用 H 的不变量的 L 的 $L'= L^H$ 子域表示。 A 的 $A_{(L')}$ 除的指数表示，因此与 $p$ 互质。到定理 6，我们在$L'$的布劳尔群中有$[L : L'][A_{(L')}] = 0$。由此得出$[A_{(L')}] = 0$和域$L'$分裂的A。然后我们VIII中的应用推论2，p. 283；由此可见，除 $[L': K]$ 的指标因此不能被$p$整除。

#### 推论 3 {#alg-viii-s16-thm-6-cor-3 .statement tag=00JU}

令$p$为素数数，令K为特征$p$的完美域。设A是K上有限次数的中心单代数。那么$p$不是A的除指标。

让我们证明 K 的布劳尔群不包含阶 $p$ 的任何元素。 有限次数的K的每个伽罗瓦扩张M是完美域（V, §7, No. 1，p. 36，命题2）。因而，取第 $p$ 个幂就是群 $M^*$ 中的自同构。由此可见，乘法乘$p$是群$H^2$(Gal(M$/K$)$,M^*$)的自同构，与Br(M$/K$)同构的。

因而，[A] 的阶与 $p$ 互质，并且通过推论 2，其指标不能被 $p$ 整除。

#### 注 {#alg-viii-s16-n11-rem-1 .statement tag=00JV}

通过考虑四元数代数的张量积，可以用中心K，指数2和任意大的指标（cf.VIII，p. 371，构造域， 习题 7 和 8)。

$*$相反，如果 K 是 $p$-adic 域的有限伽罗瓦扩张或形式幂级数的域超过有限域，则指数的中央单代数 K 上的有限次数等于其指标 (VIII, p. 332, 习题 17, e))。$*$

### 习题{#alg-viii-s16-exercises}

参见[习题为 § 16](exercises/s16/)。
