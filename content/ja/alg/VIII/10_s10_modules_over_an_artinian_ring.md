---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 10
section_title: Modules over an Artinian Ring
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.173-A VIII.181
pdf_pages: 0190-0198
extraction: native
subsections:
    - "no": 1
      title: The Radical of an Artinian Ring
      page: 173
      pdf_page: 190
    - "no": 2
      title: Modules over an Artinian Ring
      page: 174
      pdf_page: 191
    - "no": 3
      title: Projective Modules over an Artinian Ring
      page: 175
      pdf_page: 192
statements: 12
exercises: 11
content_sha256: 85c98a77b998678259c1eadca7c8a4e87286b0f6b877441465d2f6112addd458
translated_from: content/en/alg/VIII/10_s10_modules_over_an_artinian_ring.md
translation_method: google
source_content_sha256: f88ff60a0976a0441aed75f5328135625983a714fc53ed6dc1504425eb26923f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: 0f3c964a2b5cb283ef9a1bf03ad6d5d0adfe45c3318f3276abdad0ef90d0fcd1
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 10。 加群アルティン環

### 1. アルティン環中根基

#### 命題 1 {#alg-viii-s10-prop-1 .statement tag=00C5}

A を左アルティン的環とします。 根基 $\mathfrak{r}$ of A is 最大の nilpotent two-sided ideal of A, and 環 $A/\mathfrak{r}$ is 半単純.

We know (VIII, p. 156, 定理 1) that every nilpotent two-sided ideal of A is contained in $\mathfrak{r}$. $\mathfrak{r}$ がゼロであることを証明しましょう。 Since 環 A is 左アルティン的 and 数列 of two-sided ideals $\mathfrak{r}^n$ is 減少する, there exists 整数 $p\geqslant 0$ such that we have $\mathfrak{r}^p=\mathfrak{r}^{p+1}$. Since A is アルティン, A-加群 $A_s$ has 有限長 (VIII, p. 6, 定理 1) and is therefore ネーター. The left ideal $\mathfrak{r}^p$ is therefore finitely generated. By Nakayama’s 補題 (定理 2 of VIII, p. 158), it follows that $\mathfrak{r}^p= 0$.

環 $A/\mathfrak{r}$ には根基 (VIII、p. 155、命題 5) がありません。 左アルティン的なので、半単純 (VIII、p. 154、命題 4) です。

#### 系 1 {#alg-viii-s10-prop-1-cor-1 .statement tag=00C6}

環は、それが左アルティン的であり、0 以外の零の両側イデアルを持たない場合に限り、半単純です。

半単純環は左アルティン的で、根基はありません (VIII、p. 154、命題 4)。従って、0 以外の零意の両側イデアルはありません。 逆は命題 1 から続きます。

#### 系 2 {#alg-viii-s10-prop-1-cor-2 .statement tag=00C7}

左アルティン的環 A では、根基は元 $x$ で構成され、A のすべての $a$ に対して ax が零になります。

A が左アルティン的の場合、根基は冪能の両側イデアル (命題 1) です。左のゼロ理想はすべて、ジェイコブソンの定理 (VIII、p. 156、定理 1) によって根基に含まれます。 系 2が続きます。

### 2. 加群アルティン環

#### 命題 2 {#alg-viii-s10-prop-2 .statement tag=00C8}

A を左アルティン的環とします。 A-加群 M ごとに、次のプロパティは同等です。

(i) M は半単純です。

(ii) M には根基がありません。

(iii) M は A の根基 $\mathfrak{r}$ によって消滅します。

(i) は (ii) を意味することがわかります (VIII、p. 153、命題 3)。一方、$\mathfrak{r}M$ は M (VIII、p. 158、命題 6) の根基に含まれるため、(ii) は (iii) を意味します。

A-加群 M が $\mathfrak{r}$ によって全滅したとします。 環 $A/\mathfrak{r}$ を加群と見ることができます。さて、環 $A/\mathfrak{r}$ は半単純 (VIII, p. 173, 命題 1) であり、半単純環を超えるすべての加群は半単純 (VIII, p. 138, 命題 4）。従って、M は環 $A/\mathfrak{r}$ よりも半単純加群であり、環 A よりもなおさらです。従って、(iii) は (i) を意味します。

#### 系 {#alg-viii-s10-n2-cor-1 .statement tag=00C9}

A を左アルティン的環とします。 A-加群 M ごとに、M の根基は $\mathfrak{r}M$ に等しくなります。

M 含む $\mathfrak{r}M$ の根基 $\mathfrak{R}(M)$ (VIII、p. 158、命題 6)。さらにA-加群$M/\mathfrak{r}M$は$\mathfrak{r}$によって全滅します。従って、命題 2 には根基がなく、$\mathfrak{R}(M)\subset \mathfrak{r}M$ (VIII, p. 152, 系 1, c)) を意味します。

#### 命題 3 {#alg-viii-s10-prop-3 .statement tag=00CA}

A と B を A から B までの環と $f$ 準同型とし、B の $f(A)$ の和集合と $f(A)$ の交換子環 $f(A)'$ によって B が生成されるようにします。 M を左B-加群とします。 スカラー (II, §1, No. 13, p. 221) の制限によって M から推定される環 A が左アルティン的または A-加群 $f_*(M)$ のいずれかが有限生成されるとします。 すると$\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$になります。

S を単純B-加群とします。 A が左アルティン的または A-加群 $f_*(S)$ のいずれかが有限生成されるとします。 $f_*(S)$には根基が無いことを証明します。すべての $b\in f(A)'$ について、ホモテティー $b_S$ は A-加群 $f_*(S)$ の自己準同型であるため、$\mathfrak{R}_A(f_*(S))$ (VIII、p. 152、命題 1) が保持されます。 B は $f(A)\cup f(A)'$ によって生成されるため、根基 $\mathfrak{R}_A(f_*(S))$ は S の B-部分加群であるため、0 または S に等しくなります。$f_*(S)$ が有限生成A-加群である場合、$\mathfrak{R}_A(f_*(S))\not=f_*(S)$ (VIII, p. 153, 命題 2) になります。 環 A が左アルティン的の場合、$\mathfrak{R}_A(f_*(S)) =f(\mathfrak{r})S$ が得られます。ここで、$\mathfrak{r}$ は A の根基 (VIII、p. 174、系の命題 2) であり、$\mathfrak{r}$ は nilpotent であるため、 A の両面イデアル (VIII、p. 173、命題 1) の場合、できないは $S =f(\mathfrak{r})S$ になります。従って、どちらの場合も $\mathfrak{R}_A(f_*(S)) = 0$ になります。

$u$ を M から単純な M モジュール S への非零 B-線型写像とします。写像 $u$ は全射です。従って、$f_*(M)$ が有限に生成される場合、$f_*(S)$ も有限に生成されます。 命題 3 の仮定の下では、A-加群 $f_*(S)$ には根基がなく、$u$ は $f_*(M)$ から $f_*(S)$ までの A-線型写像です。従って、$u$ 含む $\mathfrak{R}_A(f_*(M))$ の核命題 VIII の 1、p. 152。 $u$は任意なので、$\mathfrak{R}_A(f_*(M))\subset \mathfrak{R}_B(M)$になります。

#### 系 {#alg-viii-s10-n2-cor-2 .statement tag=00CB}

A に対して A を可換環 、B を代数とします。A が環 A がアルティンであるか、B が有限生成A-加群であるとします。すると$\mathfrak{R}(A)B\subset \mathfrak{R}(B)$になります。

命題 3 により、根基 $\mathfrak{R}_A(B_s)$ は $\mathfrak{R}_B(B_s)$ に含まれます。これは、環 B の根基に他なりません。さらに、VIII、p. 158 の命題 6 により、$\mathfrak{R}(A)B\subset \mathfrak{R}_A(B_s)$ が得られます。 系が続きます。

### 3. 射影加群アルティン環

#### 命題 4 {#alg-viii-s10-prop-4 .statement tag=00CC}

左アルティン的環上のすべての加群には突起カバーがあります。

A を左アルティン的環、M を A 上の加群とします。A の根基 $\mathfrak{r}$ は冪能の両側イデアルであり、環 $A/\mathfrak{r}$ は半単純 (VIII, p. 173, 命題 1)。したがって、$A/\mathfrak{r}$加群 $M/\mathfrak{r}M$ は射影であることがわかります。 主張は、VIII、p. 164 の命題 11 から続きます。

#### 命題 5 {#alg-viii-s10-prop-5 .statement tag=00CD}

A を左アルティン的環とし、$\mathfrak{r}$ を根基とします。

a) P を射影 A-加群とします。 P から $P/\mathfrak{r}P$ までの標準写像を $u$ で表します。そして、$(P, u)$は$P/\mathfrak{r}P$の投影カバーです。特に、A-加群 P は、$P/\mathfrak{r}P$ が存在する場合に限り、有限に生成されます。

b) M を環 $A/\mathfrak{r}$ 以上加群とします。次に、A-加群として表示される M には、投影されたカバーがあります。 $(P, u)$ がそのような射影カバーである場合、移行から商になるとき、$u$ 誘導する同型は $P/\mathfrak{r}P$ から M になります。さらに、M が単純な場合に限り、P は分解不可能です。

c) M と $M'$ を加群環 $A/\mathfrak{r}$ とする。 $(P, u)$ と $(P', u')$ を A-加群 M と $M'$ の射影カバーとする。この場合、M と $M'$ は、P と $P'$ が同型である場合に限り、同型になります。

A の根基 $\mathfrak{r}$ は、冪能の両側イデアル (VIII、p. 173、命題 1) です。 Assertion a) therefore follows from Corollary 1 of VIII, p. 163 and Remark 2 of VIII, p. 161.

主張 b) を証明しましょう。 M の射影カバー $(P, u)$ の存在は、$P/\mathfrak{r}P$ の命題 4 と同型から、VIII、p. 162 の命題 9 の M に続きます。 環 $A/\mathfrak{r}$ は半単純なので、この環上の加群は、単純な場合に限り、分解不可能です。 最後の主張は、VIII、p. 160 の系 2 から続きます。

c)を証明しましょう。 $f$ を P から $P'$ までの同型とします。それは $P/\mathfrak{r}P$ から $P'/\mathfrak{r}P'$ まで誘導する同型 $\overline{f}$ です。 b) により、これらの商はそれぞれ M および $M'$ と同型です。 したがって、M は $M'$ と同型です。 逆に、VIII、p. 161の命題8により、Mから$M'$、持ち上げから同型、$\widetilde{f}$の同型$f$ごとに、Pから$P'$まで$f\circ u=u'\circ \widetilde{f}$になります。

#### 系 {#alg-viii-s10-n3-cor-1 .statement tag=00CE}

射影 A-加群の各類 P で、加群 $P/\mathfrak{r}P$ の類 $\varphi (P)$ を環 $A/\mathfrak{r}$ に関連付けます。 環 $A/\mathfrak{r}$ 上のすべての加群 (それぞれ有限生成加群) の類は、射影 A-加群 (有限生成射影のそれぞれ) の一意の類 P に対して、形 $\varphi (P)$ になります。 A-加群）。

A を左アルティン的環とし、$\mathfrak{r}$ を根基とします。 Denote the set of classes of simple A-modules by $\mathscr{S}$; it is finite (VIII, p. 51). VIII、p. 174 の命題 2 により、半単純環 $A/\mathfrak{r}$ 上の単純加群の類の集合と正規に識別できます。 すべての $\lambda \in \mathscr{S}$ について、$S_{\lambda}$ を類の $\lambda$ の単純A-加群とし、選ぶを $S_{\lambda}$ の射影カバー $(P_{\lambda}, u_{\lambda})$ (VIII、p. 175、命題 4) とします。 命題 5 までに、A-加群 $P_{\lambda}$ は射影的で分解不可能であり、$u_{\lambda}$ 定義する同型は $P_{\lambda}/\mathfrak{r}P_{\lambda}$ から $S_{\lambda}$ までです。 さらに、P が射影で分解不可能な A-加群である場合、P が $P_{\lambda}:$ と同型であるような一意の $\lambda \in \mathscr{S}$ が存在します。これは、$P/\mathfrak{r}P$ が $S_{\lambda}$ と同型であるような一意の $\lambda \in \mathscr{S}$ です。

#### 命題 6 {#alg-viii-s10-prop-6 .statement tag=00CF}

A を左アルティン的環とし、$\mathfrak{r}$ を根基とします。 P を射影 A-加群とします。

a) A-加群 $\overline{P}= P/\mathfrak{r}P$ は半単純であり、A-加群 P は $\bigoplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ と同型です。

b) $(Q_i)_{i\in I}$ を、直和 P を持つ P の非分解射影部分加群の族とする。すると、$\lambda \in \mathscr{S}$ ごとに、集合 $I(\lambda )$ の$i\in I$ の基数が$Q_i$ が $P_{\lambda}$ と同型であるようにする。 $[P :\lambda ]$。

$\overline{P}$ が半単純であるという事実は、命題 2 (VIII, p. 174) からわかります。 A-加群 $Q =\oplus_{\lambda\in\mathscr{S}}P^{([P:\lambda])}_{\lambda}$ は射影です。 $P_{\lambda}/\mathfrak{r}P_{\lambda}$ は $S_{\lambda}$ と同型であるため、商 $Q/\mathfrak{r}Q$ は $\oplus_{\lambda\in\mathscr{S}}S^{([P:\lambda])}_{\lambda}$、つまり $\overline{P}= P/\mathfrak{r}P$ と同型です。 命題 5 までに、A-加群 P と Q は同型になります。

射影的で分解不可能な部分加群と直和 P の族 $(Q_i)_{i\in I}$ が与えられたとします。命題 5 までに、A-加群 $Q_i/\mathfrak{r}Q_i$ はすべての $i\in I$ に対して単純です。 $\lambda \in \mathscr{S}$ については、$Q_i/\mathfrak{r}Q_i$ が $S_{\lambda}$ と同型であるように、$i\in I$ の $I(\lambda )$ 集合によって表され、したがって $P_{\lambda}/\mathfrak{r}P_{\lambda}$ となります。また、$i\in I$ の集合であるため、$Q_i$ は $P_{\lambda}$ と同型です。 $\overline{P}= P/\mathfrak{r}P$ は $(Q_i/\mathfrak{r}Q_i)_{i\in I}$ 家族の直和なので、VIII, p. 32 の 1 つである定理による Card(I($\lambda$ )) $= [P :\lambda ]$ があります。

#### 例 {#alg-viii-s10-n3-exa-1 .statement tag=00CG}

P を $A_s$ とします。 $\lambda \in \mathscr{S}$ については、単純A-加群 $S_{\lambda}$ の交換子環の反対側の体を $D_{\lambda}$ で表し、$S_{\lambda}$ の次元を体 $D_{\lambda}$ よりも右ベクトル空間として見ます。 $m(\lambda )$。 $m(\lambda )$ は重複度 $[A_s/\mathfrak{r}A_s:\lambda ]$ (VIII、p. 143、命題 11) に等しいことがわかっています。従って、A-加群 $A_s$ は $\oplus_{\lambda\in\mathscr{S}}P^{m(\lambda)}_{\lambda}$ と同型です。

### 練習問題 {#alg-viii-s10-exercises}

[§ 10 に対して練習問題](exercises/s10/)を参照してください。
