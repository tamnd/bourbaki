---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 2
section_title: Root system of a split semi-simple Lie algebra
lang: ja
source: lie-vii-ix
book_pages: 77-86, 226-229
pdf_pages: 0085-0094, 0234-0237
extraction: native
subsections:
    - "no": 1
      title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
      page: 77
      pdf_page: 85
    - "no": 2
      title: ROOTS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 78
      pdf_page: 86
    - "no": 3
      title: INVARIANT BILINEAR FORMS
      page: 83
      pdf_page: 91
    - "no": 4
      title: THE COEFFICIENTS N$_{\boldsymbol{\alpha \beta }}$
      page: 83
      pdf_page: 91
statements: 28
exercises: 11
content_sha256: 9ca67d7db62af7dc216717e8e64721a101d17007f0299be6e0a1d49dcaafce59
translated_from: content/en/lie/VIII/02_s2_root_system_of_a_split_semi_simple_lie.md
translation_method: google
source_content_sha256: 5b8fba70b72c8f243ecb19eff11bd99a4fc4e1594703137b927fa6344b3f9e7f
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: cf8067d7cb6150d064f7b8eb3d447c2bc230fc258d51d39a9d546bca0ab32238
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 2。 根系/分裂半単純リー代数

### 1. 分裂半単純リー代数

#### 定義 1 {#lie-viii-s2-def-1 .statement tag=00YK}

$\mathfrak{g}$ を半単純リー代数とします。すべての $x\in \mathfrak{h}$ について ad$_{\mathfrak{g}}x$ が三角形化可能である場合、$\mathfrak{g}$ のカルタン部分代数 $\mathfrak{h}$ は分裂と呼ばれます。 半単純リー代数に分裂カルタン部分代数がある場合、半単純リー代数は分割可能と呼ばれます。 分裂半単純リー代数は対 $(\mathfrak{g},\mathfrak{h})$ で、$\mathfrak{g}$ は半単純リー代数 、$\mathfrak{h}$ は $\mathfrak{g}$ の分裂カルタン部分代数です。

#### 注意 1 {#lie-viii-s2-n1-rem-1 .statement tag=00YL}

$\mathfrak{g}$ を $\mathfrak{g}$ の半単純リー代数、$\mathfrak{h}$ カルタン部分代数とします。すべての $x\in \mathfrak{h}$ について、ad$_{\mathfrak{g}}x$ は半単純 (第 2 章、VII, §2, no. 4) です。したがって、$\mathfrak{h}$ が分裂であるということは、ad$_{\mathfrak{g}}x$ がすべての $x\in \mathfrak{h}$ に対して対角化可能であることを意味します。

#### 注意 2 {#lie-viii-s2-n1-rem-2 .statement tag=00YM}

$k$ が代数的に閉じている場合、すべての半単純リー代数 $\mathfrak{g}$ は分割可能であり、$\mathfrak{g}$ のすべてのカルタン部分代数は分裂です。 $k$ が代数的に閉じていない場合、分割不可能な半単純リー代数 (Exerc. $2a$)$)$ が存在します。さらに、$\mathfrak{g}$ が分割可能である場合、分裂ではない$\mathfrak{g}$ のカルタン部分代数が存在する可能性があります (例: $2b$)$)$。

#### 注意 3 {#lie-viii-s2-n1-rem-3 .statement tag=00YN}

$\mathfrak{g}$ を半単純リー代数、$\mathfrak{h}$ カルタン部分代数の $\mathfrak{g}$、$\rho$ を $\rho (\mathfrak{h})$ が対角化できるような $\mathfrak{g}$ の有限次元単射関数表現とします。 Then ad$_{\mathfrak{g}}x$ is diagonalizable for all $x\in \mathfrak{h}$ (Chap. VII, §2, no. 1, Example 2), so $\mathfrak{h}$ is splitting.

#### 注意 4 {#lie-viii-s2-n1-rem-4 .statement tag=00YO}

(§3, no. 3、提案 10 の修正) $\mathfrak{h},\mathfrak{h}'$ が $\mathfrak{g}$ の分裂カルタン部分代数である場合、$\mathfrak{h}$ を $\mathfrak{h}'$ に変換する $\mathfrak{g}$ の初等自己同型が存在することがわかります。

#### 注意 5 {#lie-viii-s2-n1-rem-5 .statement tag=00YP}

$\mathfrak{g}$ を還元的なリー代数とします。次に、$\mathfrak{g}=\mathfrak{c}\times \mathfrak{s}$ ここで、$\mathfrak{c}$ は $\mathfrak{g}$ の中心で、$\mathfrak{s}=\mathscr{D}\mathfrak{g}$ は半単純です。 $\mathfrak{g}$ のカルタン部分代数は形の部分代数 $\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$ で、$\mathfrak{h}'$ は $\mathfrak{s}$ のカルタン部分代数です (第 VII, §2, no. 1 章、提案 2)。次に、$\mathfrak{h}'$ が $\mathfrak{s}$ に対して分裂である場合、$\mathfrak{h}$ は分裂と呼ばれます。これは明らかに、分割可能な定義または還元可能な分裂代数につながります。

### 2. 根/分裂半単純リー代数

この数において、$(\mathfrak{g},\mathfrak{h})$は分裂半単純リー代数を表します。

任意の $\lambda \in \mathfrak{h}^*$ については、$\mathfrak{g}^{\lambda}(\mathfrak{h})$ で表すか、単に $\mathfrak{g}^{\lambda}$ で、$\lambda$ を基準とした $\mathfrak{g}$ の主要な部分空間 (cf. 章VII, §1, no. 3) で表します。 $\mathfrak{g}^0=\mathfrak{h}$ (第 VII, §2, no. 1、提案 4)、$\mathfrak{g}$ は $\mathfrak{g}^{\lambda}$ (第 VII, §1, no. 3、提案 8 および 9) の直和、$\mathfrak{g}^{\lambda}$ は $x\in \mathfrak{g}$ の集合であることを思い出してください。すべての $h\in \mathfrak{h}$ は $[h, x] =\lambda (h)x$ (第 2 章 VII, §2, no. 4、コリント 1)、$\mathfrak{g}$ の $\mathfrak{h}$ の重みは $\mathfrak{h}$ では $\mathfrak{g}^{\lambda}\not= 0$ の線型形式 $\lambda$ です。 (VII, §1, no. 1章)。

#### 定義 2 {#lie-viii-s2-def-2 .statement tag=00YQ}

$(\mathfrak{g},\mathfrak{h})$の根は、$\mathfrak{g}$の$\mathfrak{h}$の非ゼロの重みです。

$R(\mathfrak{g},\mathfrak{h})$、または単に R、$(\mathfrak{g},\mathfrak{h})$ の根の集合で表します。私たちは持っています

$$
\mathfrak{g}=\mathfrak{h}\oplus \bigoplus_{\alpha\in R}\mathfrak{g}^{\alpha}
$$

#### 命題 1 {#lie-viii-s2-prop-1 .statement tag=00YR}

$\alpha ,\beta$ を $(\mathfrak{g},\mathfrak{h})$ の根とし、$\langle \cdot ,\cdot \rangle$ を $\mathfrak{g}($ 上の非縮退不変対称双線形形式とします。たとえば、$\mathfrak{g})$ の殺害形です。

(i) $\alpha +\beta \not= 0,\mathfrak{g}^{\alpha}$ と $\mathfrak{g}^{\beta}$ が直交する場合。 $\langle \cdot ,\cdot \rangle$ ～ $\mathfrak{g}^{\alpha}\times \mathfrak{g}^{-\alpha}$ の制限は非退化です。 $\langle \cdot ,\cdot \rangle$ ～ $\mathfrak{h}$ の制限は非退化です。

(ii) $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ と $h\in \mathfrak{h}$ とします。それから$[x, y]\in \mathfrak{h}$と

$$
\langle h,[x, y]\rangle =\alpha (h)\langle x, y\rangle
$$

主張 (i) は、第 1 章の提案 10 (iii) の特定のケースです。 VII, §1, no. 3。 $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ と $h\in \mathfrak{h}$ の場合、$[x, y]\in \mathfrak{g}^{\alpha-\alpha}=\mathfrak{h}$ があり、

$$
\langle h,[x, y]\rangle =\langle [h, x], y\rangle =\langle \alpha (h)x, y\rangle =\alpha (h)\langle x, y\rangle
$$

#### 定理 1 {#lie-viii-s2-thm-1 .statement tag=00YS}

$\alpha$を$(\mathfrak{g},\mathfrak{h})$の根とします。

(i) ベクトル空間 $\mathfrak{g}^{\alpha}$ は次元 1 のものです。

(ii) $\mathfrak{h}$ のベクトル部分空間 $\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}]$ は次元 1 のものです。含む一意元 $H_{\alpha}$ は $\alpha (H_{\alpha}) = 2$ となります。

(iii) ベクトル部分空間 $\mathfrak{s}_{\alpha}=\mathfrak{h}_{\alpha}+\mathfrak{g}^{\alpha}+\mathfrak{g}^{-\alpha}$ は、$\mathfrak{g}$ の嘘部分代数です。

(iv) $X_{\alpha}$ が $\mathfrak{g}^{\alpha}$ の非ゼロ元である場合、$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ のような一意の $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ が存在します。 $\varphi$ を、$X_+$ ～ $X_{\alpha},X_-$ ～ $X_{-\alpha}$、および $H$ ～ $H_{\alpha}$ を取る、$\mathfrak{s}\mathfrak{l}(2, k)$ から $\mathfrak{g}$ までの線形写像とします。すると、$\varphi$はリー代数$\mathfrak{s}\mathfrak{l}(2, k)$からリー代数$\mathfrak{s}_{\alpha}$の同型になります。

a) $h_{\alpha}$ を、すべての $h\in \mathfrak{h}$ に対して $\alpha (h) =\langle h_{\alpha}, h\rangle$ となるように、$\mathfrak{h}$ の一意元とします。提案 $1, [x, y] =\langle x, y\rangle h_{\alpha}$ により、すべての $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ に対して。一方、$\langle \mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}\rangle  \not= 0$。したがって$\mathfrak{h}_{\alpha}= [\mathfrak{g}^{\alpha},\mathfrak{g}^{-\alpha}] =kh_{\alpha}$です。

b) 選ぶ $x\in \mathfrak{g}^{\alpha},y\in \mathfrak{g}^{-\alpha}$ は $\langle x, y\rangle = 1$ となるため、$[x, y] =h_{\alpha}$ となります。 $[h_{\alpha}, x] =\alpha (h_{\alpha})x, [h_{\alpha}, y] =-\alpha (h_{\alpha})y$ を思い出してください。 $\alpha (h_{\alpha}) = 0$ の場合、$kx+ky+kh_{\alpha}$ は $\mathfrak{g}$ の冪能部分代数 $\mathfrak{t}$ であることがわかります。 $h_{\alpha}\in [\mathfrak{t},\mathfrak{t}]$ であるため、ad$_{\mathfrak{g}}h_{\alpha}$ は nilpotent です (Chap. I, §5, no. 3、Th. 1)。ad$_{\mathfrak{g}}h_{\alpha}$ は非ゼロの半単純であるため、これは不合理です。 ということで$\alpha (h_{\alpha})\not= 0$。 したがって、$\alpha (H_{\alpha}) = 2$ のような一意の $H_{\alpha}\in \mathfrak{h}_{\alpha}$ が存在し、これは (ii) を証明します。

c) 選ぶ $\mathfrak{g}^{\alpha}$ の非ゼロ元 $X_{\alpha}$。 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ ($[X_{\alpha},\mathfrak{g}^{-\alpha}] =\mathfrak{h}_{\alpha}$ から $b$ まで)$)$ となるような $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ が存在します。それから

$$
[H_{\alpha}, X_{\alpha}] =\alpha (H_{\alpha})X_{\alpha}= 2X_{\alpha},[H_{\alpha}, X_{-\alpha}] =-\alpha (H_{\alpha})X_{-\alpha}=-2X_{-\alpha}
$$

$$
[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}
$$

したがって、$kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$は$\mathfrak{g}$の部分代数であり、$\mathfrak{s}\mathfrak{l}(2, k)$から$kX_{\alpha}+kX_{-\alpha}+kH_{\alpha}$までの線形写像$\varphi$であり、$\varphi (X_+) =X_{\alpha},\varphi (X_-) =X_{-\alpha}$、$\varphi (H) =H_{\alpha}$はリー代数の同型になります。

d) dim$\mathfrak{g}^{\alpha}>1$ と仮定します。 $y$ を $\mathfrak{g}^{-\alpha}$ の非ゼロ元とします。 $\langle y, X_{\alpha}\rangle = 0$ となるような $\mathfrak{g}_{\alpha}$ の非ゼロ元 $X_{\alpha}$ が存在します。 c) と同様に選ぶ $X_{-\alpha}$ を考慮し、$\mathfrak{s}\mathfrak{l}(2, k)$ から $\mathfrak{g}$ までの表現 $\rho :u \rightarrow$ と$_{\mathfrak{g}}\varphi (u)$ を検討します。我々は持っています

$$
\rho (H)y= [\varphi (H), y] = [H_{\alpha}, y] =-2y
$$

$$
\rho (X_+)y= [\varphi (X_+), y] = [X_{\alpha}, y] =\langle X_{\alpha}, y\rangle h_{\alpha}= 0
$$

したがって、$y$ は、重み $-2$ の $\rho$ に対してプリミティブであり、矛盾する §1, no. 2 の Prop. 2 です。これは(i)を証明します。

e) 主張 (iii) は c) の帰結になります。一方、$X_{\alpha}$ が $\mathfrak{g}^{\alpha}$ の非ゼロ元である場合、c) で構築された元 $X_{-\alpha}$ は、$\mathfrak{g}^{-\alpha}= 1$ から $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ となるように、$\mathfrak{g}^{-\alpha}$ の一意元になります。 (iv)の最後の主張はc)の帰結です。 Q.E.D.

$h_{\alpha},H_{\alpha},\mathfrak{s}_{\alpha}$ という表記は、以下でもそのまま使用されます。 ($h_{\alpha}$ を定義するには、Killing 形式と等しい $\langle \cdot ,\cdot \rangle$ を取ります。) $X_{\alpha}$ が $\mathfrak{g}^{\alpha}$ の非ゼロ要素である場合、Th の同型性 $\varphi$ は次のようになります。 1 と、$\mathfrak{g}$ 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現 $u \rightarrow$ ad$_{\mathfrak{g}}\varphi (u)$ は、$X_{\alpha}$ に関連付けられていると言われます。

#### 系 {#lie-viii-s2-n2-cor-1 .statement tag=00YT}

$\Phi$ を $\mathfrak{g}$ の殺害形とします。 $a, b\in \mathfrak{h}$ 全員にとって、

$$
\Phi (a, b) =\sum_{\gamma\in R}\gamma (a)\gamma (b)
$$

確かに、広告 $a$.ad $b$ はそれぞれの $\mathfrak{g}^{\gamma}$ を安定させ、その制限から $\mathfrak{g}^{\gamma}$ はホモテティー で比率は $\gamma (a)\gamma (b)$ です。 $\gamma \not= 0$の場合は$\mathfrak{g}^{\gamma}= 1$を暗くします。

#### 命題 2 {#lie-viii-s2-prop-2 .statement tag=00YU}

$\alpha , \beta \in R$ にしましょう。

(i) $\beta (H_{\alpha})\in \mathbf{Z}$。

(ii) $\Phi$ が $\mathfrak{g},\Phi (H_{\alpha}, H_{\beta})\in \mathbf{Z}$ の殺害形を示す場合。

$X_{\alpha}$ を $\mathfrak{g}^{\alpha}$ の非ゼロ元とし、$\rho$ を $X_{\alpha}$ に関連付けられた $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現とします。 $\rho (H)$の固有値は0、$\beta (H_{\alpha})$は$\beta \in R$です。したがって、(i) は §1, no. 2、Cor.提案 2 の主張 (ii) は (i) および Cor. Thの。 1.Q.E.D.

$\mathfrak{g}^{\alpha},X_{-\alpha}$ のゼロ以外の要素を $\alpha \in R,X_{\alpha}$ 、$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ となるような $\mathfrak{g}^{-\alpha}$ の要素、および $X_{\alpha}$ に関連付けられた $\mathfrak{g}$ 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現を $\rho$ とします。 $\pi$ を $\rho ($§1, no. 4 と互換性のある $\mathfrak{g}$ の $\mathbf{S}\mathbf{L}(2, k)$ の表現とします。 2)。 Since ad $X_{\alpha}$ is nilpotent (Chap. VII, §1, no. 3, Prop. 10 (iv)), $\pi (e^{X_+}) =e^{adX_{\alpha}}$ is an elementary automorphism of $\mathfrak{g}$. 同様に、$\pi (e^{X_-}) =$ $e^{adX_{-\alpha}}$ は $\mathfrak{g}$ の基本自己同型です。 したがって、$\pi (\mathbf{S}\mathbf{L}(2, k))\subset$ Aut$_e(\mathfrak{g})$ となります。 §1, no. 5の記法$\theta (t)$を利用します。 $t\in k^*$には、

$$
\theta_{\alpha}(t) =\pi (\theta (t)) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}} \tag{1}
$$

#### 補題 1 {#lie-viii-s2-lem-1 .statement tag=00YV}

(i) $h\in \mathfrak{h},\theta_{\alpha}(t).h=h-\alpha (h)H_{\alpha}$ 全員に対して。

(ii) すべての$\beta \in R,\theta_{\alpha}(t)(\mathfrak{g}^{\beta}) =\mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$。

(iii) $\alpha , \beta \in R,\beta -\beta (H_{\alpha})\alpha \in R$ の場合。

$h\in \mathfrak{h}$ にしましょう。 $\alpha (h) = 0, [X_{\alpha}, h] = [X_{-\alpha}, h] = 0$なら、$\theta_{\alpha}(t).h=h$。一方、§1, no. 5の公式(5)は$\theta_{\alpha}(t).H_{\alpha}=-H_{\alpha}$であることを示しています。これにより、主張 (i) が証明されます。したがって、$\theta_{\alpha}(t)^2|\mathfrak{h}=$ 同上。 $x\in \mathfrak{g}^{\beta}$ と $h\in \mathfrak{h}$ の場合、

$$
[h, \theta_{\alpha}(t)x] =\theta_{\alpha}(t).[\theta_{\alpha}(t)h, x]-\beta (\theta_{\alpha}(t)h).\theta_{\alpha}(t)x
$$

$$
= (\beta (h)-\alpha (h)\beta (H_{\alpha})).\theta_{\alpha}(t)x
$$

$$
= (\beta -\beta (H_{\alpha})\alpha )(h).\theta_{\alpha}(t)x
$$

だから$\theta_{\alpha}(t)x\in \mathfrak{g}^{\beta-\beta(H_{\alpha})\alpha}$。これは(ii)を証明します。 主張 (iii) は (ii) から続きます。

#### 定理 2 {#lie-viii-s2-thm-2 .statement tag=00YW}

(i) 集合 $R = R(\mathfrak{g},\mathfrak{h})$ は $\mathfrak{h}^*$ の約根系です。

(ii) $\alpha \in R$ とします。 $\mathfrak{h}^*$ から $\mathfrak{h}^*$ までの写像 $s_{\alpha ,H_{\alpha}}:\lambda  \rightarrow \lambda -\lambda (H_{\alpha})\alpha$ は、$s(\alpha ) =-\alpha$ と $s(R) = R$ のような $\mathfrak{h}^*$ の固有の反映 $s$ です。 すべての $t\in k^*$ に対して、$s$ は $\theta_{\alpha}(t)|\mathfrak{h}$ の転置です。

まず、R 生成する $\mathfrak{h}^*$、$h\in \mathfrak{h}$ がすべての $\alpha \in R$ に対して $\alpha (h) = 0$ である場合、$\mathfrak{g}$ の中心は零であるため、$h= 0$ となり、したがって $h= 0$ になります。 定義、$0\notin R$までに。 $\alpha \in R$ にしましょう。 $\alpha (H_{\alpha}) = 2,s=s_{\alpha ,H_{\alpha}}$ は $s(\alpha ) =-\alpha$ のような反映であるため。次に、補題 1 (iii) によって $s(R) = R$、すべての $\beta \in R$ に対して $\beta (H_{\alpha})\in \mathbf{Z}$ (提案 2 (i))。これは、R が $\mathfrak{h}^*$ の根系であることを示しています。 $h\in \mathfrak{h}$ と $\lambda \in \mathfrak{h}^*$ のすべてについて、

$$
\langle s(\lambda ), h\rangle =\langle \lambda -\lambda (H_{\alpha})\alpha , h\rangle =\langle \lambda , h-\alpha (h)H_{\alpha}\rangle =\langle \lambda , \theta_{\alpha}(t)h\rangle
$$

したがって、$s$ は $\theta_{\alpha}(t)|\mathfrak{h}$ の転置です。最後に、根系 R が減少することを示します。 $\alpha \in R$と$y\in \mathfrak{g}^{2\alpha}$としましょう。 $3\alpha  \notin R$ (章 VI, §1, no. 3、提案 $8$)$, [X_{\alpha}, y] = 0$ 以降。一方、$[X_{-\alpha}, y]\in \mathfrak{g}^{-\alpha+2\alpha}=\mathfrak{g}^{\alpha}=kX_{\alpha}$ なので、$[X_{\alpha},[X_{-\alpha}, y]] = 0$;したがって

$$
4y= 2\alpha (H_{\alpha})y= [H_{\alpha}, y] =-[[X_{\alpha}, X_{-\alpha}], y] = 0
$$

つまり$y= 0$と$\mathfrak{g}^{2\alpha}= 0$です。他の語では、$2\alpha$は根ではありません。 Q.E.D.

同一視する $\mathfrak{h}$ は、$\mathfrak{h}^{**}$ と正規化されます。第 72 章の記法とVI, §1, no. 1、Th によって次のようになります。 2(ii)、

$\alpha \in R$全員に対して$H_{\alpha}=\alpha^{\vee}$。 (2)

したがって、$H_{\alpha}$ は、$\mathfrak{h}$ の形根系 $R^{\vee}$ が R の逆になります。

$(\mathfrak{g},\mathfrak{h})$ の $R(\mathfrak{g},\mathfrak{h})$ 根系とします。反射$s_{\alpha ,H_{\alpha}}$を単に$s_{\alpha}$と表記します。ワイル群、群の重み、コクセター 数 $. .$。 $R(\mathfrak{g},\mathfrak{h})$のワイル群、群、重み、コクセター数$. .$と呼ばれます。 $(\mathfrak{g},\mathfrak{h})$の。第 2 章のように。 VI, §1, no. 1 では、ワイル群は $\mathfrak{h}^*$ だけでなく、構造の輸送によって $\mathfrak{h}$ にも動作していると考えられるため、$s_{\alpha}=\theta_{\alpha}(t)|\mathfrak{h}$ になります。 $\theta_{\alpha}(t)$ は $\mathfrak{g}$ の基本自己同型であるため、次のようになります。

#### 系 {#lie-viii-s2-n2-cor-2 .statement tag=00YX}

$\mathfrak{h}$ で動作する、$(\mathfrak{g},\mathfrak{h})$ のワイル群の各元は、$\mathfrak{g}$ の基本自己同型の制限から $\mathfrak{h}$ です。

この結果の逆については、§5, no. 2、提案 4 を参照してください。

#### 注意 1 {#lie-viii-s2-n2-rem-1 .statement tag=00YY}

If $\mathfrak{h}_{\mathbf{Q}}$ (resp. $\mathfrak{h}^*_{\mathbf{Q}}$) denotes the $\mathbf{Q}$-vector subspace of $\mathfrak{h}$ (resp. $\mathfrak{h}^*$) generated by the $H_{\alpha}$ (resp. the $\alpha$ ), where $\alpha \in R$, then $\mathfrak{h}$ (resp. $\mathfrak{h}^*$) can be identified canonically with $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$ (resp. with $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}k$) and $\mathfrak{h}^*_{\mathbf{Q}}$ can be identified with the dual of $\mathfrak{h}_{\mathbf{Q}}$ (Chap. VI, §1, no. 1, Prop. 1). $\mathfrak{h}_{\mathbf{Q}}$ と $\mathfrak{h}^*_{\mathbf{Q}}$ を、$\mathfrak{h}$ と $\mathfrak{h}^*($代数の正規の $\mathbf{Q}$ 構造と呼びます。 II, §8, no. 1、デフォルト。 1)。 $\mathfrak{h}$のベクトル部分空間、$\mathfrak{h}$の線型形式などの$\mathbf{Q}$-合理性について言及する場合、別の意味でこれらの構造、〜でない限りを意味します。 $R(\mathfrak{g},\mathfrak{h})$ のワイル チャンバー、またはファセットについて言及するときは、$\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ または $\mathfrak{h}^*_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ で作業し、それを $\mathfrak{h}_{\mathbf{R}}$ と $\mathfrak{h}^*_{\mathbf{R}}$ で表します。

#### 注意 2 {#lie-viii-s2-n2-rem-2 .statement tag=00YZ}

$\mathfrak{h}$ 定義するの根系 $R^{\vee}$ は、$\mathfrak{h}$ 上の非縮退対称双線形形式 $\beta$ (第 VI, §1, no. 1 案、提案 3)、つまり形 $(a, b) \rightarrow$ $\sum_{\alpha\in R}\langle \alpha , a\rangle \langle \alpha , b\rangle$ です。コルによって。 Thさんへ。 1、この形はちょうど制限です

形から $\mathfrak{h}$ を殺害します。 $\beta |\mathfrak{h}_{\mathbf{Q}}\times \mathfrak{h}_{\mathbf{Q}}$ から $\mathfrak{h}_{\mathbf{Q}}\otimes_{\mathbf{Q}}\mathbf{R}$ の拡大は、正の非退化です (VI, §1, no. 1 章、提案 3)。 一方、$\mathfrak{g}$の殺害形の制限から$\mathfrak{h}$の$\mathfrak{h}^*$の逆形が、Rの正準双線形形式$\Phi_R$であることがわかります（VI, §1, no. 12章）。

$(\mathfrak{g}_1,\mathfrak{h}_1), (\mathfrak{g}_2,\mathfrak{h}_2)$ を分裂半単純リー代数、$\varphi$ 同型を $\mathfrak{g}_1$ から $\mathfrak{g}_2$ までとし、$\varphi (\mathfrak{h}_1) =\mathfrak{h}_2$ とします。 構造の輸送までに、写像の転置$\varphi |\mathfrak{h}_1$には$R(\mathfrak{g}_2,\mathfrak{h}_2)$から$R(\mathfrak{g}_1,\mathfrak{h}_1)$がかかります。

#### 命題 3 {#lie-viii-s2-prop-3 .statement tag=00Z0}

$\mathfrak{g}$ を $\mathfrak{g}$ の半単純リー代数、$\mathfrak{h}_1$、$\mathfrak{h}_2$ 分裂カルタン部分代数とします。 $\mathfrak{h}^*_1$ から $\mathfrak{h}^*_2$ までは $R(\mathfrak{g},\mathfrak{h}_1)$ から $R(\mathfrak{g},\mathfrak{h}_2)$ までかかる同型が存在します。

(より正確な結果については、提案 10 の§3, no. 3 および提案 5 の§5, no. 3 を参照してください)。

Let $k'$ be 代数閉包 of $k,\mathfrak{g}'=\mathfrak{g}\otimes_kk',\mathfrak{h}'_i=\mathfrak{h}_i\otimes_kk'$.すると、$R(\mathfrak{g}',\mathfrak{h}'_i)$は、$\mathfrak{h}^*_i$から$\mathfrak{h}^*_i\otimes_kk'={\mathfrak{h}'_i}^*$までの写像$\lambda  \rightarrow \lambda \otimes 1$の下の$R(\mathfrak{g},\mathfrak{h}_i)$の像になります。章著。 VII, §3, no. 2、木曜日。 1、$\mathfrak{h}'_1$から$\mathfrak{h}'_2$までの$\mathfrak{g}'$の自己同型が存在するため、${\mathfrak{h}'_1}^*$から${\mathfrak{h}'_2}^*$まで$R(\mathfrak{g}',\mathfrak{h}'_1)$から$R(\mathfrak{g}',\mathfrak{h}'_2)$までの同型$\varphi$が存在します。次に、$\varphi |\mathfrak{h}^*_1$ は $R(\mathfrak{g},\mathfrak{h}_1)$ から $R(\mathfrak{g},\mathfrak{h}_2)$ になり、したがって $\mathfrak{h}^*_1$ から $\mathfrak{h}^*_2$ になります。 Q.E.D.

提案 3 を考慮すると、$(\mathfrak{g},\mathfrak{h})$ の根系は、同型まで、$\mathfrak{h}$ ではなく、$\mathfrak{g}$ にのみ依存します。同様に、重み $. .$ のワイル群、群も同様です。 $(\mathfrak{g},\mathfrak{h})$の群、群、重み$. .$は、言葉を乱用して単にワイル群、群と呼ばれます。 $\mathfrak{g}$ (cf. §5, no. 3、注意 2) の。 $\mathfrak{g}$ のディンキングラフが型 $A_l$ または $B_l,. .$ の場合。 (cf. Chapter VI, §4, no. 2、Th. 3)、$\mathfrak{g}$ は型 $A_l$ または $B_l,. .$ であると言われます。

Recall that, if $\alpha$ and $\beta$ are linearly independent roots, the set of $j\in \mathbf{Z}$ such that $\beta +j\alpha \in R$ is an interval $[-q, p]$ of $\mathbf{Z}$ containing 0, with $p-q=$ $-\langle \beta , \alpha^{\vee}\rangle =-\beta (H_{\alpha})$ (Chap. VI, §1, no. 3, Prop. 9).

#### 命題 4 {#lie-viii-s2-prop-4 .statement tag=00Z1}

$\alpha$ と $\beta$ を線形独立である根とします。 $p$ (それぞれ $q$) を最大の整数 $j$ として、$\beta +j\alpha$ (それぞれ $\beta -j\alpha$ ) が根となるようにします。

(i) $\mathfrak{g}$ のベクトル部分空間 $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ は、次元 $p+q+ 1$ の単純な $\mathfrak{s}_{\alpha}$ モジュールです。

(ii) $\alpha +\beta$ が根の場合、$[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$。

$X_{\alpha}$ (それぞれ $x$) を $\mathfrak{g}^{\alpha}$ (それぞれ $\mathfrak{g}^{\beta+p\alpha}$) の非ゼロ元とします。それから

$$
[X_{\alpha}, x]\in \mathfrak{g}^{\beta+(p+1)\alpha}= 0
$$

$$
[H_{\alpha}, x] = (\beta (H_{\alpha}) +p\alpha (H_{\alpha}))x= (-p+q+ 2p)x= (p+q)x
$$

したがって、$x$ は、$X_{\alpha}$ に関連付けられた $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現に対する重み $p+q$ のプリミティブです。しかし、$\mathfrak{s}\mathfrak{l}(2, k$) モジュール $\sum_{-q\leq j\leq p}\mathfrak{g}^{\beta+j\alpha}$ は次元 $p+q+ 1$ です。したがって、それは簡単です (§1, no. 2、提案 2)。 $\alpha +\beta \in R$ の場合、$p\geq 1$ なので、$\mathfrak{g}^{\beta}$ の元は原始的ではないため、$[X_{\alpha},\mathfrak{g}^{\beta}]\not= 0$ になります。 $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}]\subset$ $\mathfrak{g}^{\alpha+\beta}$ なので、ついに $[\mathfrak{g}^{\alpha},\mathfrak{g}^{\beta}] =\mathfrak{g}^{\alpha+\beta}$ であることがわかります。

#### 注意 3 {#lie-viii-s2-n2-rem-3 .statement tag=00Z2}

思い出してください、チャプター。 VI, §1, no. 3、コル。提案 9 の整数 $p+q+ 1$ は値 $1,2,3,4$ しか取れません。

#### 注意 4 {#lie-viii-s2-n2-rem-4 .statement tag=00Z3}

$(\mathfrak{g},\mathfrak{h})$ を $\mathfrak{g},\mathfrak{g}'=\mathscr{D}\mathfrak{g}$、$\mathfrak{h}'=\mathfrak{h}\cap \mathfrak{g}'$ の分解的簡約リー代数、$\mathfrak{c}$ 中心とします。次に$\mathfrak{h}=\mathfrak{c}\times \mathfrak{h}'$、$\mathfrak{h}^*$のベクトル部分空間と同一視する$\mathfrak{h}^{'*}$です。 $\lambda \not= 0$ のような任意の $\lambda \in \mathfrak{h}^*$ では、$\lambda$ を基準とした主要な部分空間 $\mathfrak{g}^{\lambda}$ は ${\mathfrak{g}'}^{\lambda|\mathfrak{h}'}$ に等しくなります。 $\mathfrak{g}$ の $\mathfrak{h}$ の非ゼロ重みは、$(\mathfrak{g},\mathfrak{h})$ の根と呼ばれます。すべての根は $\mathfrak{c}$ に消えます。 $R(\mathfrak{g},\mathfrak{h})$ 集合の根または $(\mathfrak{g},\mathfrak{h})$ で表します。正規的には $R(\mathfrak{g}',\mathfrak{h}')$ で識別できます。 $\alpha \in R(\mathfrak{g},\mathfrak{h})$ にしましょう。 半単純の場合と同様に、$\mathfrak{g}$の$\mathfrak{s}\mathfrak{l}(2, k)$の定義する$h_{\alpha},H_{\alpha}$、$\mathfrak{s}_{\alpha}$、同型$\mathfrak{s}\mathfrak{l}(2, k)\rightarrow \mathfrak{s}_{\alpha}$、表現が$\alpha$に関連付けられます。

### 3. 不変双線形形式

#### 命題 5 {#lie-viii-s2-prop-5 .statement tag=00Z4}

$(\mathfrak{g},\mathfrak{h})$ を分裂半単純リー代数、$\Phi$ を $\mathfrak{g}$ 上の不変対称双線形形式、W を $(\mathfrak{g},\mathfrak{h})$ のワイル群とします。この場合、$\Phi$ から $\mathfrak{h}$ の制限 $\Phi '$ は W のもとで不変です。さらに、$\Phi$ が非縮退であれば、$\Phi '$ も同様です。

$\alpha \in R$、$X_{\alpha}$ をゼロ以外の $\mathfrak{g}^{\alpha},\rho$ の元、$\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}(2, k)$ の関連する表現、および $\mathfrak{g}$ の $\mathbf{S}\mathbf{L}(2, k)$ の表現を $\pi$ 表現とします。 $\rho$。したがって、$\Phi$ は $\rho$ の下で不変であり、したがって $\pi ($§1, no. 4 の下でも不変です)。特に、$\Phi '$ は $\theta_{\alpha}(t)|\mathfrak{h}$ (no. 2) の下で不変であり、したがって W の下で不変です。 最後の主張は提案 1 (i) から導き出されます。

#### 命題 6 {#lie-viii-s2-prop-6 .statement tag=00Z5}

$(\mathfrak{g},\mathfrak{h})$ を分裂半単純リー代数、$\Phi$ を $\mathfrak{g}$ 上の非縮退不変対称双線形形式とします。すべての $\alpha \in R$ について、$X_{\alpha}$ を $\mathfrak{g}^{\alpha}$ の非ゼロ元とします。 $(H_i)_{i\in I}$ を $\mathfrak{h}$ の基底とし、$\mathfrak{h}$ の $(H'_i)_{i\in I}$ 基底を$\Phi (H_i, H'_j) =\delta_{ij}$ とします。 $\mathfrak{g}$ (第 I, §3, no. 7 章) を囲む代数の $\Phi$ に関連付けられたカシミール元は、次のようになります。

$$
\sum\frac{1}{\Phi(X_{\alpha}, X_{-\alpha})}X_{\alpha}X_{-\alpha}+\sum H_iH'_i
$$

$\alpha \in Ri\in I$

確かに、提案 $1,\Phi (H_i, X_{\alpha}) =\Phi (H'_i, X_{\alpha}) = 0$ はすべての $i\in I,\alpha \in R$ に対して、$\Phi (\frac{1}{\Phi(X_{\alpha},X_{-\alpha})}X_{\alpha}, X_{-\beta})=\delta_{\alpha \beta}$ はすべての $\alpha , \beta \in R$ に対して行われます。

### 4. ザ係数 N$_{\boldsymbol{\alpha \beta }}$

この数を、再び $(\mathfrak{g},\mathfrak{h})$ 分裂半単純リー代数で表します。

#### 補題 2 {#lie-viii-s2-lem-2 .statement tag=00Z6}

$\alpha \in R$ 全員にとって、次のような家族 $(X_{\alpha})_{\alpha\in R}$ が存在します。

$X_{\alpha}\in \mathfrak{g}^{\alpha}$と$[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$。

$R_1$ を、$R = R_1\cup (-R_1)$ と $R_1\cap (-R_1) =\emptyset$ となるような R の部分集合とします。 $\alpha \in R_1$、選ぶの場合は、$\mathfrak{g}^{\alpha}$ の任意の非ゼロ元 $X_{\alpha}$。 $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ のような固有の $X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ が存在します (Th. 1 (iv))。それから

$$
[X_{-\alpha}, X_{\alpha}] =H_{\alpha}=-H_{-\alpha}.Q.E.D
$$

$(X_{\alpha})_{\alpha\in R}$ が 2 の補題の 1 つのファミリー 満たす条件である場合、最も一般的なファミリー 満たすであるこれらの条件は $(t_{\alpha}X_{\alpha})_{\alpha\in R}$ で、すべての $\alpha \in R$ に対して $t_{\alpha}\in k^*$ と $t_{\alpha}t_{-\alpha}= 1$ が入ります。

この数の残りでは、補題 2 の族満たす条件を $(X_{\alpha})_{\alpha\in R}$ で表します。 $\mathfrak{g}$ 上の非縮退不変対称双線形形式を $\langle \cdot ,\cdot \rangle$ で表します。

すべての $x\in \mathfrak{g}$ は形で一意に記述することができます

$$
x=h+\sum_{\alpha\in R}\mu_{\alpha}X_{\alpha}(h\in \mathfrak{h}, \mu_{\alpha}\in k)
$$

このような 2 つの元の括弧は、次の公式を使用して計算できます。

$$
[h, X_{\alpha}] =\alpha (h)X_{\alpha}
$$

$\alpha +\beta  \notin R\cup  \{0\}$の場合は0

$[X_{\alpha}, X_{\beta}] =-H_{\alpha}$ $\alpha +\beta = 0$ の場合

$N_{\alpha \beta}X_{\alpha+\beta}$ $\alpha +\beta \in R$ の場合

$N_{\alpha \beta}$ は $k$ の非ゼロ元です。

#### 補題 3 {#lie-viii-s2-lem-3 .statement tag=00Z7}

$\alpha \in R$ 全員にとって、

$$
\langle X_{\alpha}, X_{-\alpha}\rangle =-\frac{1}{2}\langle H_{\alpha}, H_{\alpha}\rangle
$$

確かに、

$$
2\langle X_{\alpha}, X_{-\alpha}\rangle =\langle \alpha (H_{\alpha})X_{\alpha}, X_{-\alpha}\rangle =\langle [H_{\alpha}, X_{\alpha}], X_{-\alpha}\rangle
$$

$$
=\langle H_{\alpha},[X_{\alpha}, X_{-\alpha}]\rangle =-\langle H_{\alpha}, H_{\alpha}\rangle
$$

#### 補題 4 {#lie-viii-s2-lem-4 .statement tag=00Z8}

$\alpha , \beta \in R$ を $\alpha +\beta \in R$ となるようにします。 $p$ (それぞれ $q$) を最大の整数 $j$ として、$\beta +j\alpha \in R$ (それぞれ $\beta -j\alpha \in R$) とします。それから、

$$
N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}=-p(q+ 1) \tag{3}
$$

$$
N_{-\alpha ,\alpha+\beta}\langle H_{\beta}, H_{\beta}\rangle =-N_{-\alpha ,-\beta}\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle \tag{4}
$$

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}= (q+ 1)^2 \tag{5}
$$

$\rho$ を、$X_{\alpha}$ によって定義される $\mathfrak{g}$ 上の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現とします。 元 $e=X_{\beta+p\alpha}$ は、重み $p+q$ のプリミティブです (提案 4 (i))。置く

$e_n=(-n1)$! $n\geq 0$の場合は$^n\rho (X_-)^ne$。

§1の提案1により、

(広告$X_{\alpha}$)$e_p= (q+ 1)e_{p-1}$

(広告$X_{-\alpha}$)(広告$X_{\alpha}$)$e_p=-p(q+ 1)e_p$。

$e_p$ は $\mathfrak{g}^{\beta}$ の非ゼロ元であるため、これは (3) を証明します。

形 $\langle \cdot ,\cdot \rangle$ は不変なので、

$$
\langle [X_{-\alpha}, X_{\alpha+\beta}], X_{-\beta}\rangle =-\langle X_{\alpha+\beta},[X_{-\alpha}, X_{-\beta}]\rangle
$$

それで

$$
N_{-\alpha ,\alpha+\beta}\langle X_{\beta}, X_{-\beta}\rangle =-N_{-\alpha ,-\beta}\langle X_{\alpha+\beta}, X_{-\alpha-\beta}\rangle
$$

補題 3 を考慮すると、これは (4) を証明します。

$\langle \cdot ,\cdot \rangle$ から $\mathfrak{h}$ の制限は、ワイル群 (提案 5) の下で非縮退かつ不変です。 同一視する $\mathfrak{h}$ と $\mathfrak{h}^*$ は、この制限によって行われます。 $\gamma \in R,H_{\gamma}$ が $2\gamma /\langle \gamma , \gamma \rangle$ と同一視される場合 (VI, §1, no. 1、補題 2 章)。したがって、すべての $\gamma , \delta \in R$ について、

$$
\langle \gamma , \gamma \rangle \langle H_{\delta}, H_{\delta}\rangle
$$

$$
\overline{\langle\delta , \delta\rangle}=\overline{\langle H_{\gamma}, H_{\gamma}\rangle} \tag{6}
$$

さて、Chap. VI, §1, no. 3、提案 10、

$$
\frac{\langle\alpha + \beta , \alpha + \beta\rangle}{\langle\beta , \beta\rangle}=\frac{q + 1}{p} \tag{7}
$$

したがって、(3)、(4)、(6)、(7) により、

$$
N_{\alpha ,\beta}N_{-\alpha ,-\beta}=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{\langle H_{\beta}, H_{\beta}\rangle}{\langle H_{\alpha+\beta}, H_{\alpha+\beta}\rangle}
$$

$$
=-N_{\alpha ,\beta}N_{-\alpha ,\alpha+\beta}\frac{q + 1}{p}= (q+ 1)^2
$$

#### 定義 3 {#lie-viii-s2-def-3 .statement tag=00Z9}

$(\mathfrak{g},\mathfrak{h})$ のシュバレー 系は、次のような家族 $(X_{\alpha})_{\alpha\in R}$ です。

(i) $\alpha \in R$ 全員に対して $X_{\alpha}\in \mathfrak{g}^{\alpha}$;

(ii) $\alpha \in R$ 全員に対して $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$。

(iii) $\mathfrak{h}$ の $-1$ に等しく、すべての $\alpha \in R$ に対して $X_{\alpha}$ から $X_{-\alpha}$ を取る$\mathfrak{g}$ から $\mathfrak{g}$ までの線形写像は、$\mathfrak{g}$ の自己同型です。

この定義の拡大を$(\mathfrak{g},\mathfrak{h})$が分裂の場合に還元すると明らかになります。

$(\mathfrak{g},\mathfrak{h})$ に対する Chevalley 系が存在することを示します (§4, no. 4、提案 5 の補正)。

#### 命題 7 {#lie-viii-s2-prop-7 .statement tag=00ZA}

$(X_{\alpha})_{\alpha\in R}$ を $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系とします。 補題 4 の記法を保持します。次に、$N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$ と $N_{\alpha ,\beta}=\pm (q+ 1)$ を $\alpha , \beta , \alpha +\beta \in R$ にします。

$\varphi$ を Def で考慮される $\mathfrak{g}$ の自己同型とします。 3(iii)。それから

$$
N_{-\alpha ,-\beta}X_{-\alpha-\beta}= [X_{-\alpha}, X_{-\beta}] = [\varphi (X_{\alpha}), \varphi (X_{\beta})] =\varphi ([X_{\alpha}, X_{\beta}])
$$

$$
=\varphi (N_{\alpha ,\beta}X_{\alpha+\beta}) = N_{\alpha ,\beta}X_{-\alpha-\beta}
$$

だから$N_{-\alpha ,-\beta}= N_{\alpha ,\beta}$。 (5)までに$N_{\alpha ,\beta}=\pm (q+ 1)$になりました。

#### 命題 8 {#lie-viii-s2-prop-8 .statement tag=00ZB}

$(X_{\alpha})_{\alpha\in R}$ を $(\mathfrak{g},\mathfrak{h})$ のシュバレー 系とします。 M を $\mathfrak{h}$ 含むと $H_{\alpha}$ の $\mathbf{Z}$ サブモジュールとし、$R^{\vee}$ の重みの群に含まれるとします。 $\mathfrak{g}_{\mathbf{Z}}$ を、M と $X_{\alpha}$ によって生成された $\mathfrak{g}$ の $\mathbf{Z}$ サブモジュールとします。この場合、$\mathfrak{g}_{\mathbf{Z}}$ は $\mathfrak{g}$ の $\mathbf{Z}$-嘘部分代数であり、$\mathfrak{g}_{\mathbf{Z}}\otimes_{\mathbf{Z}}k$ から $\mathfrak{g}$ までの正規の写像は同型です。

$\alpha , \beta \in R$ が $\alpha +\beta \in R$ となる場合、$N_{\alpha ,\beta}\in \mathbf{Z}$ (提案 7)。一方、$\alpha \in R$と$h\in M$の場合は、$\alpha (h)\in \mathbf{Z}$になります（VI, §1, no. 9章）。これは、$\mathfrak{g}_{\mathbf{Z}}$が$\mathfrak{g}$の$\mathbf{Z}$嘘部分代数であることを証明します。一方、M は、階数 dim$\mathfrak{h}($代数のフリー アーベル群です。 VII, §3、木曜日。 1) したがって、$\mathfrak{g}_{\mathbf{Z}}$ は、階数 dim$\mathfrak{g}$ の無料のアーベル群です。これは最後の主張を意味します。

### 練習問題 {#lie-viii-s2-exercises}

[§ 2 に対して練習問題](exercises/s2/)を参照してください。
