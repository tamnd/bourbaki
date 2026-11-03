---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 9
section_title: The formula of Hermann Weyl
lang: ja
source: lie-vii-ix
book_pages: 152-159, 253-260
pdf_pages: 0160-0167, 0261-0268
extraction: native
subsections:
    - "no": 1
      title: CHARACTERS OF FINITE DIMENSIONAL $\mathfrak{g}$-MODULES
      page: 152
      pdf_page: 160
    - "no": 2
      title: DIMENSIONS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 154
      pdf_page: 162
    - "no": 3
      title: MULTIPLICITIES OF WEIGHTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 156
      pdf_page: 164
    - "no": 4
      title: DECOMPOSITION OF TENSOR PRODUCTS OF SIMPLE $\mathfrak{g}$-MODULES
      page: 157
      pdf_page: 165
statements: 12
exercises: 16
content_sha256: 23123b98a7a96049ec50127eb65985a969d21e338f407fd28ca525ee08017a3a
translated_from: content/en/lie/VIII/09_s9_the_formula_of_hermann_weyl.md
translation_method: google
source_content_sha256: 16e58934b12a0ac3234fd1dee9446b6558b2edb33a94c1d55bbd2fbd906273b2
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0ec4286d8930ef73459d397809141b239265772a23e251f9e33c3cb8302f5f31
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 9。ヘルマン・ワイルの公式

この段落では、§6 と §7 の一般的な記法を保持します。

### 1. 有限次元 $\mathfrak{g}$ モジュールの指標

$(e^{\lambda})_{\lambda\in\mathfrak{h}^*}$ を環 $\mathbf{Z}[\mathfrak{h}^*]$ の標準基底とします。 因子の離散トポロジーの $\mathfrak{h}^*$ から $\mathbf{Z}$ までのすべての写像積位相のうち空間 $\mathbf{Z}^{\mathfrak{h}^*}$ を与えます。 $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$ の場合、ファミリー $(\varphi (\nu )e^{\nu})_{\nu\in\mathfrak{h}^*}$ は合計可能であり、

$$
\varphi =\sum_{\nu\in\mathfrak{h}^*}\varphi (\nu )e^{\nu}
$$

$\mathbf{Z}\langle P\rangle$ を $\varphi \in \mathbf{Z}^{\mathfrak{h}^*}$ の集合とし、そのサポートは形 $\nu -P_+$ の集合の有限和集合に含まれます。ここで、$\nu \in \mathfrak{h}^*$ です。 次に$\mathbf{Z}[P]\subset \mathbf{Z}\langle P\rangle  \subset \mathbf{Z}^{\mathfrak{h}^*}$。 Define on $\mathbf{Z}\langle P\rangle$ a ring structure extending that of $\mathbf{Z}[P]$ by putting, for $\varphi , \psi \in \mathbf{Z}\langle P\rangle$ and $\nu \in \mathfrak{h}^*$,

$$
(\varphi \psi )(\nu ) =\sum_{\mu\in\mathfrak{h}^*}\varphi (\mu)\psi (\nu -\mu)
$$

($\varphi$ と $\psi$ のサポートによって満足される条件を考慮すると、家族 $(\varphi (\mu)\psi (\nu -\mu))_{\mu\in\mathfrak{h}^*}$ には有限台があります)。 $\varphi =\sum_{\nu}x_{\nu}e^{\nu}$ と $\psi =\sum_{\nu}y_{\nu}e^{\nu}$ の場合は、$\varphi \psi =\sum_{\nu ,\mu}x_{\nu}y_\mu e^{\nu+\mu}$ です。

$\nu \in \mathfrak{h}^*$ にしましょう。 $\nu$ を正の根に変換した分割は家族 $(n_{\alpha})_{\alpha\in R_+}$ で、$n_{\alpha}$ は整数 $\geq 0$ で、$\nu =\sum_{\alpha\in R_+}n_{\alpha}\alpha$ になります。 $\nu$の分割の$\mathfrak{P}(\nu )$数を正の根に表します。我々は持っています

$$
\mathfrak{P}(\nu )>0\Leftarrow \Rightarrow \nu \in Q_+
$$

この段落では、次の $\mathbf{Z}\langle P\rangle :$ の元を K で表します

$$
K =\sum_{\gamma\in Q_+}\mathfrak{P}(\gamma )e^{-\gamma}
$$

ここで、(第 VI, §3, no. 3 章、提案 2) を思い出してください。

$$
d=\prod_{\alpha\in R_+}(e^{\alpha /2}-e^{-\alpha /2}) =\sum_{w\in W}\varepsilon (w)e^{w\rho}
$$

は、$\mathbf{Z}[P]$ の反不変式元です。

#### 補題 1 {#lie-viii-s9-lem-1 .statement tag=015T}

環 $\mathbf{Z}\langle P\rangle$ には $K.\prod_{\alpha\in R_+}(1-e^{-\alpha}) = Ke^{-\rho}d= 1$ があります。

確かに、

$$
K =\prod_{\alpha\in R_+}(e^0+e^{-\alpha}+e^{-2\alpha}+\cdots )
$$

それで

$$
Ke^{-\rho}d=\prod_{\alpha\in R_+}(1 +e^{-\alpha}+e^{-2\alpha}+\cdots )\prod_{\alpha\in R_+}(1-e^{-\alpha}) = 1
$$

#### 補題 2 {#lie-viii-s9-lem-2 .statement tag=015U}

$\lambda \in \mathfrak{h}^*$ にしましょう。 加群 $Z(\lambda ) ($§6, no. 3) は、$\mathbf{Z}\langle P\rangle$ の元である指標を認め、$d$ が得られます。チャンネル$Z(\lambda ) =e^{\lambda+\rho}$。

$\alpha_1, . . . , \alpha_q$ を $R_+$ の元と区別します。 $Z(\lambda ) ($§6 の$X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . . X_{-\alpha_q}^{n_q}\otimes 1$ 形基底、提案 6 (iii))。 $h\in \mathfrak{h}$ については、

$$
h.(X_{-\alpha_1}^{n_1}X_{-\alpha_2}^{n_2}. . .X_{-\alpha_q}^{n_q}\otimes 1)
$$

$$
= [h, X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}]\otimes 1 + (X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q})\otimes h.1
$$

$$
= (\lambda -n_1\alpha_1- \cdots  -n_q\alpha_q)(h)(X_{-\alpha_1}^{n_1}. . . X_{-\alpha_q}^{n_q}\otimes 1)
$$

したがって、$Z(\lambda )^{\lambda-\mu}$ の次元は $\mathfrak{P}(\mu)$ です。これは、ch $Z(\lambda )$ が定義されていること、$\mathbf{Z}\langle P\rangle$ の元であること、および次のことを証明します。

ch$Z(\lambda ) =\sum_\mu\mathfrak{P}(\mu)e^{\lambda-\mu}= Ke^{\lambda}$。

ここで、補題 1 を適用するだけで十分です。

#### 補題 3 {#lie-viii-s9-lem-3 .statement tag=015V}

M を、集合 $\mu-P_+$ の有限和集合にサポートが含まれる指標 ch(M) を許容する $\mathfrak{g}$ モジュールとします。 U を、$\mathfrak{g}$ の代数、U$,\lambda_0\in \mathfrak{h}^*$ の Z 中心、および Z から $k($§8 までの $\chi_{\lambda_0}$ 対応する準同型とします。 Thの1 2)。すべての $z\in Z,z_M$ がホモテティー で、比率は $\chi_{\lambda_0}(z)$ であると仮定します。 $\lambda + Q_+$ が Supp(ch M) を満たすように、$D_M$ を $\lambda \in W(\lambda_0+\rho )-\rho$ の集合とします。この場合、ch(M) は、$\lambda \in D_M$ に対する ch $Z(\lambda )$ の $\mathbf{Z}$ 線形結合になります。

Supp(ch M) が空の場合、補題はクリアです。 Supp(ch $M$)$\not=\emptyset$ と仮定します。 $\lambda$をこのサポートの極大元とし、暗い$M^{\lambda}=m$を置きます。 $(Z(\lambda ))^m$ から M への $\mathfrak{g}$ 準同型性 $\varphi$ が存在し、写像 $(Z(\lambda )^{\lambda})^m$ が $M^{\lambda}($§6, no. 3 に全単射する、提案 6 (i))。したがって、$Z(\lambda )$ の中心指標は $\chi_{\lambda_0}$ なので、$\lambda \in W(\lambda_0+\rho )-\rho ($§8, no. 5、Cor。 Thの1 2)。これは$D_M\not=\emptyset$を証明し、カード$D_M$の帰納法によって議論することができます。 L と N を $\varphi$ の核と余核とします。次に、$\mathfrak{g}$-準同型性の完全系列があります。

$$
0\rightarrow L\rightarrow (Z(\lambda ))^m\rightarrow M\rightarrow N\rightarrow 0
$$

それで

ch(M) $=-$ch(L) $+m$ ch $Z(\lambda ) +$ ch(N)

(§7, no. 7、公式 (6))。 集合 Supp(ch L) と Supp(ch N) は、集合 $\mu-P_+$ の有限和集合に含まれます。 $z\in Z,z_L$ と $z_N$ は比 $\chi_{\lambda_0}(z)$ で相似です。明らかに、$D_N\subset D_M$です。一方、$(\lambda + Q_+)\cap$Supp(ch $M$)$=\{\lambda \}$、$\lambda  \notin$Supp(ch N)なので、$\lambda  \notin D_N$と

カード$D_N<$ カード$D_M$。

一方、Lは$(Z(\lambda ))^m$の部分加群です。 $\lambda '\in D_L$ の場合、$\lambda '+ Q_+$ は補足 (ch $L$)$\subset$ 補足 ch $Z(\lambda )$ を満たすため、$\lambda \in \lambda '+ Q_+($§6, no. 1、提案 1 (ii));その結果、$D_L\subset D_M$ となります。 $L\cap (Z(\lambda )^{\lambda})^m= 0$ なので、$\lambda  \notin D_L$ があるので、

カード$D_L<$ カード$D_M$。

ここで、帰納法の仮定を適用するだけで十分です。

#### 定理 1 (H. ワイルの指標公式) {#lie-viii-s9-thm-1 .statement tag=015W}

M を有限次元の単純な $\mathfrak{g}$ 加群とし、$\lambda$ をその最高重量とします。それから

$(\sum_{w\in W}\varepsilon (w)e^{w\rho})$.ch $M =\sum_{w\in W}\varepsilon (w)e^{w(\lambda+\rho)}$.

補題 3 の記法により、M の中心指標は $\chi_{\lambda}($§6, no. 4 になります、提案 7)。したがって、補題 2 と $3,d$.ch により、M は次のような $e^{\mu+\rho}$ の $\mathbf{Z}$ 線形結合になります。

$$
\mu+\rho \in W(\lambda +\rho )
$$

一方、§7, no. 7 により、補題 $7,d$.ch M は反不変であり、その固有の最大値項は $e^{\lambda+\rho}$ であるため、定理になります。

#### 例 {#lie-viii-s9-n1-exa-1 .statement tag=015X}

$\mathfrak{g}=\mathfrak{s}\mathfrak{l}(2, k),\mathfrak{h}=kH$に乗ります。 $\alpha$ を $(\mathfrak{g},\mathfrak{h})$ の根として、$\alpha (H) = 2$ とします。 $\mathfrak{g}$ モジュール $V(m)$ には最高重量 $(m/2)\alpha$ があります。したがって、

ch(V($m$))$= (e^{(m/2)\alpha+^1_2\alpha}-e^{-(m/2)\alpha-^1_2\alpha})/(e^{^1_2\alpha}-e^{-^1_2\alpha})$

$$
=e^{-(m/2)\alpha}.(e^{(m+1)\alpha}-1)/(e^{\alpha}-1)
$$

$$
=e^{-(m/2)\alpha}(e^{m\alpha}+e^{(m-1)\alpha}+\cdots + 1)
$$

$$
=e^{(m/2)\alpha}+e^{(m-2)\alpha /2}+\cdots +e^{-(m/2)\alpha}
$$

これは、§1, no. 2、提案 2 からも簡単に導かれます。

### 2. シンプルな$\mathfrak{g}$-モジュールの次元

$\mu\in \mathfrak{h}^*$の場合、$J(e^\mu) =\sum_{w\in W}\varepsilon (w)e^{w\mu}$、cf.を入れます。 VI, §3, no. 3。

#### 定理 2 {#lie-viii-s9-thm-2 .statement tag=015Y}

E を有限次元の単純な $\mathfrak{g}$ 加群、$\lambda$ をその最高重量、$(\cdot  | \cdot )$ を $\mathfrak{h}^*$ 上の W 不変非縮退正対称双線形形式とします。次に:

$$
\prod\langle \lambda +\rho , H_{\alpha}\rangle \prod((\lambda |\alpha ))
$$

ディム E = = 1 +。

$$
_{\alpha\in R_+}\langle \rho , H_{\alpha}\rangle_{\alpha\in R_+}\overline{(\rho|\alpha)}
$$

T を不定数とします。すべての $\nu \in P$ について、$\mathbf{Z}[P]$ から $\mathbf{R}[[T]]$ までの $f_{\nu}$ 準同型で表します。これには、すべての $\mu\in P$ について $e^\mu$ から $e^{(\nu|\mu)T}$ がかかります。すると、dim E は系列 $f_{\nu}$(ch E) の定数項になります。

$\mu, \nu \in P$ の皆様には、

$$
f_{\nu}(J(e^\mu)) =\sum_{w\in W}\varepsilon (w)e^{(\nu|w\mu)T}
$$

$$
=\sum_{w\in W}\varepsilon (w)e^{(w^{-1}\nu|\mu)T}=f_\mu(J(e^{\nu}))
$$

特に、Chapter の観点から、 VI, §3, no. 3、公式 (3)、

$$
f_{\rho}(J(e^\mu)) =f_\mu(J(e^{\rho})) =e^{(\mu|\rho)T}\prod_{\alpha\in R_+}(1-e^{-(\mu|\alpha)T})
$$

したがって、設定カード(R$_+$) $= N$、

$f_{\rho}(J(e^\mu))\equiv T^N\prod_{\alpha\in R}(\mu|\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]]$)。

したがって、等式 $J(e^{\lambda+\rho}) =$ ch(E)$.J(e^{\rho})$ (Th. 1) は次のことを意味します。

$T^N\prod_{\alpha\in R_+}(\lambda +\rho |\alpha )\equiv f_{\rho}$(ch $E$)$.T^N\prod_{\alpha\in R_+}(\rho |\alpha )$ (mod $T^{N+1}\mathbf{R}[[T]]$)

それで

薄暗い$E =((\prod_{\alpha\in R_+}(\lambda +\rho |\alpha ))/((\prod_{\alpha\in R_+}(\rho |\alpha ))=\prod_{\alpha\in R_+}(1 +\frac{(\lambda|\alpha)}{(\rho|\alpha)})$。

さて、$\alpha \in R_+,\alpha$ が $H_{\alpha}$ に比例する $\mathfrak{h}_{\mathbf{R}}$ の元と識別できる場合、

$$
(\lambda +\rho |\alpha )/(\rho |\alpha ) =\langle \lambda +\rho , H_{\alpha}\rangle /\langle \rho , H_{\alpha}\rangle
$$

#### 例 1 {#lie-viii-s9-n2-exa-1 .statement tag=015Z}

no. 1 の例で、次のことがわかります。

薄暗い$V(m) =(\frac{m}{2}\alpha +\frac{\alpha}{2})(H_{\alpha})/\frac{\alpha}{2}(H_{\alpha}) =m+ 1$、

それは§1で分かりました。

#### 例 2 {#lie-viii-s9-n2-exa-2 .statement tag=0160}

$\mathfrak{g}$ を型 $G_2$ の分割可能な単純なリー代数として、第 2 章の記法を採用します。 VI、プレートIX。 $(\alpha_1|\alpha_1) = 1$ となるような W 不変の正対称形 $(\cdot  | \cdot )$ を $\mathfrak{h}^*_{\mathbf{R}}$ に与えます。それから$\rho =\varpi_1+\varpi_2$と

$$
(\varpi_1|\alpha_1) =\frac{1}{2},(\varpi_1|\alpha_2) = 0,(\varpi_1|\alpha_2+\alpha_1) =\frac{1}{2}
$$

$$
(\varpi_1|\alpha_2+ 2\alpha_1) = 1,(\varpi_1|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_1|2\alpha_2+ 3\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_1) = 0,(\varpi_2|\alpha_2) =\frac{3}{2},(\varpi_2|\alpha_2+\alpha_1) =\frac{3}{2}
$$

$$
(\varpi_2|\alpha_2+ 2\alpha_1) =\frac{3}{2},(\varpi_2|\alpha_2+ 3\alpha_1) =\frac{3}{2},(\varpi_2|2\alpha_2+ 3\alpha_1) = 3
$$

したがって、$n_1, n_2$ が整数 $\geq 0$ である場合、最高重量 $n_1\varpi_1+n_2\varpi_2$ の単純な表現の次元は次のようになります。

$$
(1 +\frac{n_1/2}{1\overline{2}})((1 +\frac{3n_2/2}{3\overline{2}})((1 +\frac{n_1/2 + 3n_2/2}{_{1\overline{2}} + \frac{3}{2}})((1 +\frac{n_1 + 3n_2/2}{1 +^{3\overline{2}}})
$$

$$
\times (1 +\frac{3n_1/2 + 3n_2/2}{_{3\overline{2}} + \frac{3}{2}})((1 +3n_1\frac{/_3}{2}2 + 3+ 3n_2)
$$

$$
= (1 +n_1)(1 +n_2)(1 +\frac{n_1 + 3n_2}{4})((1 +\frac{2n_1 + 3n_2}{5})((1 +\frac{n_1 + n_2}{2})
$$

$$
\times (1 +\frac{n_1 + 2n_2}{3})
$$

$$
(1+n_1)(1+n_2)(2+n_1+n_2)(3+n_1+2n_2)(4+n_1+3n_2)(5+2n_1+3n_2)
$$

=。

5！

特に、最高重量 $\varpi_1$ (それぞれ $\varpi_2$) の基本的な表現は、次元 7 (それぞれ 14) です。

### 3. 単純な $\mathfrak{g}$ モジュールの重みの多重度

#### 命題 1 {#lie-viii-s9-prop-1 .statement tag=0161}

$\omega \in P_{++}$ にしましょう。すべての $\lambda \in P$、$E(\omega )$ の $\lambda$ の重複度は、

$$
m_{\lambda}=\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ))
$$

Thさんより1 と補題 1、

チャンネル$E(\omega ) = Ke^{-\rho}d$ チャンネル$E(\omega ) = Ke^{-\rho}\sum_{w\in W}\varepsilon (w)e^{w(\omega+\rho)}$

それで

ch $E(\omega ) =\sum_{w\in W,\gamma\in Q_+}\varepsilon (w)\mathfrak{P}(\gamma )e^{-\rho+w(\omega+\rho)-\gamma}$

そして

$$
m_{\lambda}=\sum\varepsilon (w)\mathfrak{P}(\gamma )
$$

$w\in W,\gamma \in Q_+,\gamma =-\lambda -\rho +w(\omega +\rho )$

#### 系 {#lie-viii-s9-n3-cor-1 .statement tag=0162}

$\lambda$ が $\omega$ とは異なる $E(\omega )$ の重みである場合、

$$
m_{\lambda}=-\sum_{w\in W,w\not=1}\varepsilon (w)m_{\lambda+\rho-w\rho}
$$

$\omega = 0$ で提案 1 を適用します。 $\mu\in P$**--** $\{0\}$ の場合、次のことがわかります。

$$
0 =\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w\rho +\mu-\rho )
$$

したがって

$$
\mathfrak{P}(\mu) =-\sum_{w\in W,w\not=1}\varepsilon (w)\mathfrak{P}(\mu+w\rho -\rho ) \tag{1}
$$

提案 1 は次のことも示します

$$
m_{\lambda}=-\sum_{w\in W}\varepsilon (w)\sum_{w'\in W,w'\not=1}\varepsilon (w')\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho ) +w'\rho -\rho )
$$

$w(\omega +\rho )\not=\lambda +\rho$ 以降、すべての $w\in W ($§7、提案 5 (iii))。したがって、

$$
m_{\lambda}=-\sum_{w'\in W,w'\not=1}\varepsilon (w')\sum_{w\in W}\varepsilon (w)\mathfrak{P}(w(\omega +\rho )-(\lambda +\rho -w'\rho +\rho ))
$$

$=-\sum_{w'\in W,w'\not=1}\varepsilon (w')m_{\lambda+\rho-w'\rho}$ (プロップ$.1$)。

### 4. シンプルな $\mathfrak{g}$ モジュールの分解テンソル積

#### 命題 2 {#lie-viii-s9-prop-2 .statement tag=0163}

$\lambda , \mu\in P_{++}$ にしましょう。 $\mathscr{R}(\mathfrak{g})$ では、

$$
[\lambda ].[\mu] =\sum_{\nu\in P_{++}}m(\lambda , \mu, \nu )[\nu ]
$$

と

$$
m(\lambda , \mu, \nu ) =\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho ))
$$

$E,F$ を最高重量 $\lambda , \mu$ の有限次元単純 $\mathfrak{g}$ 加群とする。 $l_{\nu}$ を、最高重量 $\nu$ の$E\otimes F$ の同型成分の長さとします。それを示せば十分です

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (ww')\mathfrak{P}(w(\lambda +\rho ) +w'(\mu+\rho )-(\nu + 2\rho )) \tag{2}
$$

$c_1=$ ch(E) $=\sum_{\sigma\in P}m_{\sigma}e^{\sigma},c_2=$ ch(F) および $d= J(e^{\rho})$ を入力します。ここで、J は no. 2 のように定義されます。 $\sum_{\xi\in P_{++}}l_{\xi}$ch[$\xi ] =$ch(E $\otimes F$) $=c_1c_2$]

従って、後でに $d$ を乗算し、Th を使用します。 1、

$$
\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho}) =c_1J(e^{\mu+\rho}) =(\sum_{\sigma\in P}m_{\sigma}e^{\sigma})((\sum_{w\in W}\varepsilon (w)e^{w(\mu+\rho)}) \tag{3}
$$

$$
=\sum_{\tau\in P}(\sum_{w\in W}\varepsilon (w)m_{\tau+\rho-w(\mu+\rho)})e^{\tau+\rho}
$$

Now, if $\xi \in P_{++},\xi +\rho$ belongs to the chamber defined by B (Chap. VI, §1, no. 10); thus, for all $w\in W$ distinct from 1, we have $w(\xi +\rho )\notin P_{++}$. 従って、$\sum_{\xi\in P_{++}}l_{\xi}J(e^{\xi+\rho})$ の $e^{\nu+\rho}$ の係数は $l_{\nu}$ に等しくなります。 (3) を考慮すると、次のようになります。

$$
l_{\nu}=\sum_{w\in W}\varepsilon (w)m_{\nu+\rho-w(\mu+\rho)}
$$

つまり、提案 1 により、

$$
l_{\nu}=\sum_{w,w'\in W}\varepsilon (w)\varepsilon (w')\mathfrak{P}(w'(\lambda +\rho )-(\nu +\rho -w(\mu+\rho ) +\rho ))
$$

これは (2) を証明します。

#### 例 {#lie-viii-s9-n4-exa-1 .statement tag=0164}

no. 1の例に戻ります。 $\lambda = (n/2)\alpha , \mu= (p/2)\alpha$、$\nu = (q/2)\alpha$ を $n\geq p$ とします。我々は持っています

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(\frac{n}{2}\alpha +\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
-\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}+\frac{p}{2}\alpha +\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
+\mathfrak{P}(-\frac{n}{2}\alpha -\frac{\alpha}{2}-\frac{p}{2}\alpha -\frac{\alpha}{2}-\frac{q}{2}\alpha -\alpha )
$$

$$
=\mathfrak{P}(\frac{n + p-q}{2}\alpha )-\mathfrak{P}(\frac{n-p-q- 2}{2}\alpha )
$$

$n+p+q$ が 2 で割り切れない場合、または $q\geq n+p$ の場合、これは零になります。もし

$$
q=n+p-2r
$$

$r$ 整数 $\geq 0$ では、

$$
m(\lambda , \mu, \nu ) =\mathfrak{P}(r\alpha )-\mathfrak{P}((r-p-1)\alpha )
$$

従って、$r\leq p$の場合は$m(\lambda , \mu, \nu ) = 1$、$r > p$の場合は$m(\lambda , \mu, \nu ) = 0$となります。最後に、$\mathfrak{g}$ モジュール $V(n)\otimes V(p)$ は以下と同型です。

$$
V(n+p)\oplus V(n+p-2)\oplus V(n+p-4)\oplus  \cdots  \oplus V(n-p)
$$

（クレブシュ＝ゴルダン公式）。

### 練習問題 {#lie-viii-s9-exercises}

考慮されるすべての $\mathfrak{g}$ モジュールは有限次元であると仮定されます。

[§ 9 に対して練習問題](exercises/s9/)を参照してください。
