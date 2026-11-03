---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 5
section_title: Automorphisms of a semi-simple Lie algebra
lang: ja
source: lie-vii-ix
book_pages: 106-115, 233-237
pdf_pages: 0114-0123, 0241-0245
extraction: native+ocr
subsections:
    - "no": 1
      title: AUTOMORPHISMS OF A FRAMED SEMI-SIMPLE LIE ALGEBRA
      page: 106
      pdf_page: 114
    - "no": 2
      title: AUTOMORPHISMS OF A SPLIT SEMI-SIMPLE LIE ALGEBRA
      page: 107
      pdf_page: 115
    - "no": 3
      title: AUTOMORPHISMS OF A SPLITTABLE SEMI-SIMPLE LIE ALGEBRA
      page: 111
      pdf_page: 119
    - "no": 4
      title: ZARISKI TOPOLOGY ON Aut($\mathfrak{g}$)
      page: 113
      pdf_page: 121
    - "no": 5
      title: LIE GROUP CASE
      page: 115
      pdf_page: 123
statements: 25
exercises: 13
errata:
    - says: Chap. VII, §13, no. 1
      read: Chap. VIII, §13, no. 1
      why: Chapter VII has five sections and no section 13. The sentence says that the groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct, and the place that shows it is no. 1 of section 13 of this chapter, on the algebras of type $A_l$, which computes Aut$_0(\mathfrak{g}) =\varphi (\mathbf{G}\mathbf{L}(l+ 1, k))$, identifies the quotient Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$ with $\mathbf{P}\mathbf{G}\mathbf{L}(l+ 1, k)/\mathbf{P}\mathbf{S}\mathbf{L}(l+ 1, k)$, and over the reals finds it isomorphic to $\mathbf{Z}/2\mathbf{Z}$ when $l+1$ is even. Chapter VII names neither group anywhere.
content_sha256: fded43ec4243b5218be73a161ea3c5dc2fea7bc50a38814f8dd3948899e6091a
translated_from: content/en/lie/VIII/05_s5_automorphisms_of_a_semi_simple_lie.md
translation_method: google
source_content_sha256: 952a7b9240fa2d193986215a77b227fd820dee9114e1cdbfa00e8cbcdb6611b5
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: 0c8404cb8eae2e5c9ea6c4ddd231c3809a50e364b5814105c7addede85e1392f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 5。 半単純リー代数中自己同型

この段落では、$\mathfrak{g}$は半単純リー代数を表します。

### 1. 額装済み半単純リー代数の自己同型

Aut($\mathfrak{g}$) が $\mathfrak{g}$ の自己同型の群を表すこと (第 VII, §3, no. 1 章) を思い出してください。 $\mathfrak{h}$ が $\mathfrak{g}$ のカルタン部分代数である場合、$\mathfrak{h}$ を安定に残す $\mathfrak{g}$ の自己同型の Aut($\mathfrak{g},\mathfrak{h}$) 群で表します。 $\mathfrak{h}$ が分裂であると仮定し、R を $(\mathfrak{g},\mathfrak{h})$ の根系とします。 $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) の場合、$s|\mathfrak{h}$ の対偶写像は A(R) の元 (R の自己同型の群) であり、この段落ではこれを $\varepsilon (s)$ で表します。したがって

$\varepsilon :$ オート($\mathfrak{g},\mathfrak{h}$)$\rightarrow A(R)$

は群の準同型です。

R の任意の根系 R および任意の基底 B について、B を安定に保つ R の自己同型の群を Aut(R$,B$) で表します。 A(R) は Aut(R$,B$) と W(R) の半直接積であり、$A(R)/W(R)$ はディンキンの自己同型の群と正準的に同型であることを思い出してください (提案 1 のVI, §1, no. 5 章と§4, no. 2 章)。 Rのグラフ。

#### 命題 1 {#lie-viii-s5-prop-1 .statement tag=011N}

$(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B})$ をフレーム化された半単純リー代数 、R 根系を $(\mathfrak{g},\mathfrak{h})$ とします。 G を、B を安定に保つ $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) の集合とし、他の語自己同型の集合と $(\mathfrak{g},\mathfrak{h},B,(X_{\alpha})_{\alpha\in B}))$ のすべての $\alpha \in B ($ に対して $s(X_{\alpha}) =X_{\varepsilon(s)\alpha}$ とする。すると、Gへの$\varepsilon$の制限は、GからAut(R$,B$)への同型になります。

$s\in G$ であれば、$\varepsilon (s)\in$ Aut(R$,B$) であることは明らかです。一方、写像

$\varepsilon |G : G\rightarrow$オート(R$,B$)

Th による全単射です。 §4, no. 4 の 2 つ。

### 2. 自己同型/分裂半単純リー代数

E を可換群、$A =\bigoplus_{\gamma\in E}A^{\gamma}$ を E グレードの代数とします。 群 E から乗法群 $k^*$ までの任意の準同型 $\varphi$ について、$f(\varphi )$ を A から A までの $k$ 線形写像とし、各 $A^{\gamma}$ に対する制限が比でホモテティー となるようにします。 $\varphi (\gamma )$; $f(\varphi )$ はグレード代数 A の自己同型であり、$f$ はグレード代数 A の群 Hom(E$, k^*$) から自己同型の群までの準同型であることは明らかです。

$\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数、および $(\mathfrak{g},\mathfrak{h})$ の R 根系とします。 P(R) (または Q(R)) が R の重みの群 (または根基重み) を表すことを思い出してください。

$T_P=$ホム(P(R)$, k^*$)$T_Q=$ホム(Q(R)$, k^*$)。

$\mathfrak{g}=\mathfrak{g}^0+\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$ は Q(R) で評価された代数と考えることができます。前述の $T_Q$ から Aut($\mathfrak{g},\mathfrak{h}$) までの注意定義する標準準同型をこの段落では $f$ で示します。一方、Q(R)からP(R)までの標準単射定義する準同型 $T_P$から$T_Q$までを$q:$と表記します

$T_P\longrightarrow^qT_Q\longrightarrow^f$ オート($\mathfrak{g},\mathfrak{h}$)。

$s\in$ Aut($\mathfrak{g},\mathfrak{h}$) の場合、$s^*$ を Q(R) の $^t(s|\mathfrak{h})^{-1}$ の制限とします。それでは、$\varphi \in T_Q$ 全員に対して、

$$
f(\varphi \circ s^*) =s^{-1}\circ f(\varphi )\circ s \tag{1}
$$

確かに、$\gamma \in Q(R)$ と $x\in \mathfrak{g}^{\gamma}$ としましょう。次に $sx\in \mathfrak{g}^{s^*\gamma}$ と

$$
f(\varphi \circ s^*)x= (\varphi \circ s^*)(\gamma ).x=s^{-1}(\varphi (s^*\gamma )sx) = (s^{-1}\circ f(\varphi )\circ s)(x)
$$

#### 命題 2 {#lie-viii-s5-prop-2 .statement tag=011O}

数列/準同型

1 $\longrightarrow T_Q\longrightarrow^f$ Aut($\mathfrak{g},\mathfrak{h}$)$\longrightarrow^{\varepsilon}$ A(R) $\longrightarrow$ 1

正確です。

a) $\varphi \in$ カー$f$ とします。次に、すべての $\alpha \in R$ に対して $\varphi (\alpha ) = 1$ です。 R 生成する群 $Q(R),\varphi$ は $T_Q$ の単位元であるため。

b) $\varphi \in T_Q$ とします。 $f(\varphi )$～$\mathfrak{h}=\mathfrak{g}^0$の制限が正体なので、

私は$f\subset$カー$\varepsilon$です。

c) $s\in$ Ker$\varepsilon$ とします。次に、$s|\mathfrak{h}=$ ID$_{\mathfrak{h}}$ です。すべての $\alpha \in R$ に対して、$s(\mathfrak{g}^{\alpha}) =\mathfrak{g}^{\alpha}$ があり、すべての $x\in \mathfrak{g}^{\alpha}$ に対して $sx=t_{\alpha}x$ となるような $t_{\alpha}\in k^*$ が存在します。 $s\in$ Aut($\mathfrak{g}$) を条件と書くと、関係が得られます。

$t_{\alpha}t_{-\alpha}= 1$ 全員$\alpha \in R$

$\alpha , \beta , \alpha +\beta \in R$のときは$t_{\alpha}t_{\beta}=t_{\alpha+\beta}$。

これらの条件の下には、すべての $\alpha \in R$ に対して $\varphi (\alpha ) =t_{\alpha}$ となるような $\varphi \in T_Q$ が存在します (提案 19 のVI, §1, no. 6 章、コリント 2)。次に$s=f(\varphi )$。したがって、カー $\varepsilon \subset$ 私は $f$ です。

d) $\varepsilon$ 含む W(R) の下の Aut($\mathfrak{g},\mathfrak{h}$) の像 by §2, no. 2、Cor。 Thの。 2、および提案 1 による含む Aut(R$,B$)。 したがって、この像は A(R) に等しいです。

#### 系 1 {#lie-viii-s5-prop-2-cor-1 .statement tag=011P}

$(B,(X_{\alpha})_{\alpha\in B})$ を $(\mathfrak{g},\mathfrak{h})$ のフレームとします。 G をフレーミング不変のままにする $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) の集合とする。すると、Aut($\mathfrak{g},\mathfrak{h}$) は G と $\varepsilon^{-1}(W(R))$ の半直接積です。

確かに、提案 1 による $G\cap \varepsilon^{-1}(W(R)) =\{1\}$、および

オート($\mathfrak{g},\mathfrak{h}$) $= G.\varepsilon^{-1}(W(R))$

$\varepsilon$ は全射法であるため (提案 2)。

#### 系 2 {#lie-viii-s5-prop-2-cor-2 .statement tag=011Q}

群 $\varepsilon^{-1}(W(R))$ は、$(\mathfrak{g},\mathfrak{h})$ のフレームの集合で単純推移的に動作します。

実際、Aut($\mathfrak{g},\mathfrak{h}$) は、§4, no. 4 による $(\mathfrak{g},\mathfrak{h})$ のフレームの集合で推移的に動作します。 2.コル。 2 は Cor から続きます。 1.

#### 系 3 {#lie-viii-s5-prop-2-cor-3 .statement tag=011R}

B を R の基底とします。群 Ker $\varepsilon =f(T_Q)$ は、形 $(B,(X_{\alpha})_{\alpha\in B})$ の $(\mathfrak{g},\mathfrak{h})$ のフレームの集合で単純推移的に動作します。

これは提案 2 の直後の結果です。

$\alpha \in R,X_{\alpha}\in \mathfrak{g}^{\alpha},X_{-\alpha}\in \mathfrak{g}^{-\alpha}$ を $[X_{\alpha}, X_{-\alpha}] =-H_{\alpha}$ となるようにします。私たちは、初級自己同型のすべての $t\in k^*$、制限について (§2, no. 2、Th. 2) を見てきました。

$$
\theta_{\alpha}(t) =e^{adtX_{\alpha}}e^{adt^{-1}X_{-\alpha}}e^{adtX_{\alpha}}
$$

$\mathfrak{h}$ は $s_{\alpha}$ の転置です。従って、$\varepsilon (\theta_{\alpha}(t)) =s_{\alpha}$、その結果、$\theta_{\alpha}(t)\theta_{\alpha}(-1)\in$ カー$\varepsilon$ となります。

#### 補題 1 {#lie-viii-s5-lem-1 .statement tag=011S}

$\alpha \in R$と$t\in k^*$としましょう。 Q(R)から$k^*$まで$\varphi$を準同型$\lambda  \rightarrow t^{\lambda(H_{\alpha})}$とします。それから$f(\varphi ) =\theta_{\alpha}(t)\theta_{\alpha}(-1)$。

$\rho$ を $X_{\alpha}$ に関連付けられた $\mathfrak{g}$ の $\mathfrak{s}\mathfrak{l}(2, k)$ の表現とします。 $\pi$ を $\rho$ と互換性のある $\mathbf{S}\mathbf{L}(2, k)$ の表現とします。 §1, no. 5の記法$\theta (t), h(t)$を紹介します。 $\rho (H) =$ と $H_{\alpha}$ から、$\mathfrak{g}^{\lambda}$ の元は $\rho$ の重み $\lambda (H_{\alpha})$ になります。 §2までに、いいえ。 $2,\theta_{\alpha}(t)\theta_{\alpha}(-1) =\pi (\theta (t)\theta (-1)) =\pi (h(t))$。従って、$\theta_{\alpha}(t)\theta_{\alpha}(-1)$ 対 $\mathfrak{g}^{\lambda}$ の制限は、比率 $t^{\lambda(H_{\alpha})}($§1, no. 5 のホモテティー、提案 6)、従って、補題です。

#### 命題 3 {#lie-viii-s5-prop-3 .statement tag=011T}

合成準同型の像

$T_P\longrightarrow^qT_Q\longrightarrow^f$ オート($\mathfrak{g},\mathfrak{h}$)

Aut$_e(\mathfrak{g})$に収録されています。

BをRの基底とすると、$(H_{\alpha})_{\alpha\in B}$は$R^{\vee}$の基底、$\mathfrak{h}^*$の$(H_{\alpha})_{\alpha\in B}$の双対基底は群P(R)の基底となります。従って、群 $T_P$ は準同型 $\lambda  \rightarrow t^{\lambda(H_{\alpha})}(t\in k^*, \alpha \in B)$ によって生成されます。 Q(R) に対して、準同型の制限が $\varphi$ である場合、補題 1 は $f(\varphi )\in$ Aut$_e(\mathfrak{g})$ であることを証明し、したがって命題になります。

$\overline{k}$ を $k$ の代数閉包とします。 $\mathfrak{g}$ 自己同型 $s\otimes 1$ のいずれかの自己同型 $s$ $\mathfrak{g}\otimes_k\overline{k}$ に関連する写像は、Aut($\mathfrak{g}$) から Aut($\mathfrak{g}\otimes_k\overline{k}$) までの単射準同型です。 Aut$_0(\mathfrak{g})$ によって、この準同型の下で Aut$_e(\mathfrak{g}\otimes_k\overline{k})$ の逆像である Aut($\mathfrak{g}$) の通常の部分群を表します。これは、基礎体を $k$ から $\overline{k}$ に拡張することで基本となる $\mathfrak{g}$ の自己同型の集合です。 Aut$_e(\mathfrak{g})$ が $\overline{k}$ の選択から独立しており、Aut$_e(\mathfrak{g})\subset$ Aut$_0(\mathfrak{g})$ が独立していることは明らかです。 The groups Aut$_0(\mathfrak{g})$ and Aut$_e(\mathfrak{g})$ can be distinct (Chap. VII, §13, no. 1). $\mathfrak{h}$ が $\mathfrak{g}$ のカルタン部分代数である場合、

Aut$_e(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$)、Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_0(\mathfrak{g})\cap$ Aut($\mathfrak{g},\mathfrak{h}$)。

#### 補題 2 {#lie-viii-s5-lem-2 .statement tag=011U}

$\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数、および $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ とします。 $s$～$\sum_{\alpha\in R}\mathfrak{g}^{\alpha}$の制限は固有値のように1が無いとします。

次に$\varepsilon (s) = 1$。

$k$ の拡大までに、$s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$ の場合に帰着します。 The dimension of the nilspace of $s-1$ is at least dim $\mathfrak{h}$ (Chap. VII, §4, no. 4, Prop. 9). 従って、$(s-1)|\mathfrak{h}$ は無能です。 $s|\mathfrak{h}\in A(R^{\vee}),s|\mathfrak{h}$ は有限位数であるため、半単純となります（V、付録、提案 2）。 従って、$(s-1)|\mathfrak{h}= 0$ となり、$\varepsilon (s) = 1$ であることが証明されます。

#### 補題 3 {#lie-viii-s5-lem-3 .statement tag=011V}

(i) $m= (P(R) : Q(R))$ とします。 $\varphi$ が $T_Q$ の元の $m$ 番目の冪である場合、$\varphi \in q(T_P)$ です。

(ii) $k$ が代数的に閉じている場合、$q(T_P) = T_Q$。

P(R) の基底 $(\lambda_1, . . . , \lambda_l)$ と $(n_1\lambda_1, . . . , n_l\lambda_l)$ が Q(R) の基底となるような整数 $n_1\geq 1, . . . , n_l\geq 1$ が存在します。 $m=n_1. . . n_l$ があります。 $\psi \in T_Q$ に$\psi (n_1\lambda_1) =t_1, . . . , \psi (n_l\lambda_l) =t_l$ を置きます。 $i= 1, . . . , l$には、$m_i=$ $\prod_{j\not=i}n_j$を入れます。 $\chi$ を $T_P$ の元として、$\chi (\lambda_1) =t^{m_1}_1, . . . , \chi (\lambda_l) =t^{m_l}_l$ とします。それから

$$
\chi (n_i\lambda_i) =t^{m_in_i}_i=t^m_i= (\psi^m)(n_i\lambda_i)
$$

それで$\chi |Q(R) =\psi^m$。これは(i)を証明します。 $k$ が代数的に閉じている場合、$k^*$ のすべての元は、$k^*$ の元の $m$ 番目の冪であるため、$T_Q$ のすべての元は $m$ 番目になります冪/元/$T_Q$;したがって、(ii) は (i) から導かれます。

#### 命題 4 {#lie-viii-s5-prop-4 .statement tag=011W}

$f(T_Q)\subset$Aut$_0(\mathfrak{g},\mathfrak{h})$と$\varepsilon^{-1}(W(R)) =$Aut$_0(\mathfrak{g},\mathfrak{h})$があります。

a) $\varphi \in T_Q$ と $\overline{k}$ を $k$ の代数閉包とします。 Hom(P(R)$, k^*$)の補題$3,\varphi$拡大するから元まで。提案 3 により、

$f(\varphi )\otimes 1\in$ 8月$_e(\mathfrak{g}\otimes_k\overline{k},\mathfrak{h}\otimes_k\overline{k})$。

したがって、$f(\varphi )\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$、および Ker $\varepsilon \subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$ となります。

b) $\varepsilon$ 含む W(R) に基づく Aut$_e(\mathfrak{g},\mathfrak{h})$ の像 (§2, no. 2、Th. 2 の Cor.)。 a) を考慮すると、$\varepsilon^{-1}(W(R))\subset$ Aut$_0(\mathfrak{g},\mathfrak{h})$ であることがわかります。

c) Aut$_0(\mathfrak{g},\mathfrak{h})\subset \varepsilon^{-1}(W(R))$ を証明することはまだ残っている。 b) を考慮すると、$\varepsilon$(Aut$_0(\mathfrak{g},\mathfrak{h})$)$\cap$ Aut(R$,B$) を証明すれば十分です。ここで、B は R の基底、簡約する ～ $\{1\}$ を表します。

$s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ を $\varepsilon (s)\in$ Aut(R$,B$) となるようにします。 $\varepsilon (s)$ によって生成された A(R) の部分群は、R 上で軌道の有限数を持ちます。U を、基数 $r$、$\mathfrak{g}^U=\sum_{\beta\in U}\mathfrak{g}^{\beta}$ の軌道とします。 $\beta_1\in U$ とし、$\beta_i=\varepsilon (s)^{i-1}\beta_1$ を置きます

$1\leq i\leq r$、つまり $U =\{\beta_1, . . . , \beta_r\}$ です。 $X_{\beta_1}$ を 0 以外の元の $\mathfrak{g}^{\beta_1}$ とし、$1\leq i\leq r$ に $X_{\beta_i}=s^{i-1}X_{\beta_1}$ を代入します。 $s^rX_{\beta_1}=$ $c_UX_{\beta_1}$ のような $c_U\in k^*$ が存在するため、すべての $i$ に対して $s^rX_{\beta_i}=c_UX_{\beta_i}$ が存在し、その結果 $s^r|\mathfrak{g}^U=c_U.1$ になります。 $\varphi \in T_Q$ と $s'=s\circ f(\varphi )$ とします。これは、a) により、Aut$_0(\mathfrak{g},\mathfrak{h})$ の元です。 ${s'}^r|\mathfrak{g}^U=c'_U.1$ があります。

$$
c'_U=c_U\prod_{i=1}^r\varphi (\beta_i) =c_U\varphi (\sum_{i=1}^r\beta_i)
$$

$B =\{\alpha_1, . . . , \alpha_l\}$と$\sum_{i=1}^r\beta_i=\sum_{j=1}^lm^U_j\alpha_j$を入れます。 $\varepsilon (s)\in$ Aut(R$,B$) 以降、

$m^U_j$ は同じ記号の整数であり、すべてが零であるわけではありません。我々は持っています

$$
c'_U=c_U\prod_{j=1}^l\varphi (\alpha_j)^{m^U_j}
$$

これで、軌道 U ごとに $c'_U\not= 1$ となるように $\varphi$ を選択できます。実際、この簡約するは、同じ零ではなく、$t_1, . . . , t_l$ の有限の多項式数によって消滅しない $k^*$ の元 $\varphi (\alpha_1) =t_1, . . . , \varphi (\alpha_l) =t_l$ を選択することになります。このような $\varphi ,\varepsilon (s') = 1$ の選択 by 補題 2 では、

$$
\varepsilon(s)=\varepsilon(s')\varepsilon(f(\varphi))^{-1}=1.
$$

#### 系 {#lie-viii-s5-n2-cor-1 .statement tag=01J0}

— $B$ を $R$ の基底とします。 群 $\operatorname{Aut}(\mathfrak g,\mathfrak h)$ は、群 $\operatorname{Aut}(R,B)$ および $\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$ の半直接積と同型です。

これは、提案 1、コリント 1 から導き出されます。提案 2 の 1、および提案 4。

#### 注意 {#lie-viii-s5-n2-rem-1 .statement tag=011X}

$\varepsilon',\varepsilon''$を$\varepsilon$から$\operatorname{Aut}_0(\mathfrak g,\mathfrak h)$、$\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$の制限とします。 $f'$ を、$Q(R)$ から $P(R)$ までの標準単射を介して、$f$ によって誘発された $T_P$ から $\operatorname{Aut}_e(\mathfrak g,\mathfrak h)$ までの準同型とします。前で、次の可換図式を確立しました。
$$
\begin{array}{ccccccccc}
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon\ }&A(\mathbf R)&\longrightarrow&1\\
&&\uparrow&&\uparrow&&\uparrow&&\\
1&\longrightarrow&T_Q&\xrightarrow{\ f\ }&\operatorname{Aut}_0(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon'\ }&W(\mathbf R)&\longrightarrow&1\\
&&\uparrow^{q}&&\uparrow&&\uparrow&&\\
&&T_P&\xrightarrow{\ f'\ }&\operatorname{Aut}_e(\mathfrak g,\mathfrak h)&\xrightarrow{\ \varepsilon''\ }&W(\mathbf R)&\longrightarrow&1
\end{array}
$$
ここで、$q$以外の垂直矢印は標準単射を表します。最初の 2 行が正確であることがわかりました (提案 2 と 4)。 3 行目では、準同型 $\varepsilon''$ は全射法です (§2, no. 2、Th. 2 の Cor.)。その核は $f'(T_P)$ (§7、演習 26 d)) であることがわかります。

### 3. 分割可能な自己同型半単純リー代数

#### 命題 5 {#lie-viii-s5-prop-5 .statement tag=01J1}

— $\mathfrak g$ は分割可能であると仮定します。 群 $\operatorname{Aut}_0(\mathfrak g)$ は、$\mathfrak g$ のフレームの集合に対して単純推移的に動作します。

$e_1=(\mathfrak g,\mathfrak h_1,B_1,(X^1_\alpha)_{\alpha\in B_1})$、$e_2=(\mathfrak g,\mathfrak h_2,B_2,(X^2_\alpha)_{\alpha\in B_2})$を$\mathfrak g$の2つのフレームとします。 $e_2$ に変換 $e_1$ を加える $\operatorname{Aut}_0(\mathfrak g)$ の元が少なくとも 1 つ存在します (提案 1 と提案 4)。 $\overline{k}$ を $k$ の代数閉包とします。 $\mathfrak h_2\otimes_k\overline{k}$には変換$\mathfrak h_1\otimes_k\overline{k}$という$\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$の元が存在します（VII, §3, no. 2章、第1章）。 したがって、提案 4 と Cor.提案 2 の 2 では、$\mathfrak g\otimes_k\overline{k}$ のフレーム$(\mathfrak g\otimes_k\overline{k},\mathfrak h_1\otimes_k\overline{k},B_1,(X^1_\alpha)_{\alpha\in B_1})$ をフレーム$(\mathfrak g\otimes_k\overline{k},\mathfrak h_2\otimes_k\overline{k},B_2,(X^2_\alpha)_{\alpha\in B_2})$ に変換する$\operatorname{Aut}_e(\mathfrak g\otimes_k\overline{k})$ の要素$\varphi$ が存在します。 $\mathfrak h_1$ と $X^1_\alpha$ (それぞれ $\mathfrak h_2$ と $X^2_\alpha$) 生成する $\mathfrak g_1$ (それぞれ $\mathfrak g_2$) なので、$\varphi(\mathfrak g_1)=\mathfrak g_2$ があるため、$\varphi$ は形 $\psi\otimes 1$ になります。 $\psi\in\operatorname{Aut}_0(\mathfrak g)$、$\psi$ 変換 $e_1$ を $e_2$ に変換します。

#### 系 1 {#lie-viii-s5-prop-5-cor-1 .statement tag=01J2}

— $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ を $\mathfrak g$ のフレーミングとし、このフレーミングを不変のままにする $\mathfrak g$ の自己同型の $G$ 群 ($\operatorname{Aut}(R,B)$ と同型) とします。次に、$\operatorname{Aut}(\mathfrak g)$は$G$と$\operatorname{Aut}_0(\mathfrak g)$の半直接積です。

実際、$\operatorname{Aut}(\mathfrak g)$ 変換 $(\mathfrak g,\mathfrak h,B,(X_\alpha)_{\alpha\in B})$ のすべての元が $\mathfrak g$ のフレームに組み込まれます。提案 5 により、$\operatorname{Aut}_0(\mathfrak g)$ を法とする$\operatorname{Aut}(\mathfrak g)$ のすべての剰余類は、正確に 1 つの点で $G$ と一致します。

Q.E.D.

それはコルから続きます。 群 Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ は Aut(R$,B$) と識別でき、R のディンキングラフの自己同型の群と同型であることがわかります。

#### 系 2 {#lie-viii-s5-prop-5-cor-2 .statement tag=01J3}

Aut($\mathfrak{g}$) $=$ Aut$_0(\mathfrak{g})$ $\mathfrak{g}$ が型 $A_1,B_n(n\geq 2)$、$C_n(n\geq 2)$、$E_7,E_8,F_4,G_2$ の分割可能な単純なリー代数である場合。 商 Aut($\mathfrak{g}$)$/$Aut$_0(\mathfrak{g})$ は、$\mathfrak{g}$ が型 $A_n(n\geq 2)$、$D_n(n\geq 5)$、$E_6$ の場合、位数 2 になります。 $\mathfrak{g}$ が型 $D_4$ であるとき、それは $\mathfrak{S}_3$ と同型です。

これはコルからの続きです。 1と第2章VI、プレートI～IX。

#### 注意 1 {#lie-viii-s5-n3-rem-1 .statement tag=011Z}

$e_1= (\mathfrak{g},\mathfrak{h}_1,B_1,(X_{\alpha}^1)_{\alpha\in B_1}),e_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(X_{\alpha}^2)_{\alpha\in B_2})$、$e'_2= (\mathfrak{g},\mathfrak{h}_2,B_2,(Y_{\alpha}^2)_{\alpha\in B_2})$ を、$\mathfrak{g}$、$s$ (それぞれ $s'$) 元の Aut$_0(\mathfrak{g})$ と変換 $e_1$ から $e_2$ (それぞれ $e'_2$) のフレームとします。次に$s|\mathfrak{h}_1=s'|\mathfrak{h}_1$。確かに、$s^{'-1}s\in$ Aut$_0(\mathfrak{g},\mathfrak{h}_1)$ と $s^{'-1}s(B_1) = B_1$ なので、$\varepsilon (s^{'-1}s) = 1$ になります。

#### 注意 2 {#lie-viii-s5-n3-rem-2 .statement tag=0120}

X を対 $(\mathfrak{h},B)$ の集合とします。ここで、$\mathfrak{h}$ は $\mathfrak{g}$ の分裂カルタン部分代数と、$(\mathfrak{g},\mathfrak{h})$ の根系の B 基底です。 $x= (\mathfrak{h},B)$と$x'= (\mathfrak{h}',B')$がXの2つの元である場合、変換$x$を$x'$に変換する$s\in$Aut$_0(\mathfrak{g})$が存在します（提案5）、および制限$s_{x',x}$ $s$から$\mathfrak{h}$は、$s$(注意1)の選択に依存しません。特に、$x, x', x''\in X$なら$s_{x'',x'}\circ s_{x',x}=s_{x'',x}$、そして$s_{x,x}= 1$です。 集合家族数 $(h_x)_{x\in X}$ 満たす条件

$a)h_x\in \mathfrak{h}$ $x= (\mathfrak{h},B)$ の場合

$b)s_{x',x}(h_x) =h_{x'}$ $x, x'\in X$ の場合

is in a natural way ベクトル空間 $\mathfrak{h}(\mathfrak{g})$ which we ときどき call the canonical カルタン部分代数 of $\mathfrak{g}$. For $x= (\mathfrak{h},B)$ and $x'= (\mathfrak{h}',B'),s_{x',x}$ takes B to $B'$, and hence 根系 of $(\mathfrak{g},\mathfrak{h})$ to that of $(\mathfrak{g},\mathfrak{h}')$; it follows that the dual $\mathfrak{h}(\mathfrak{g})^*$ of $\mathfrak{h}(\mathfrak{g})$ is naturally equipped with 根系 $R(\mathfrak{g})$ and with 基底 $B(\mathfrak{g})$ of $R(\mathfrak{g})$. We ときどき say that $R(\mathfrak{g})$ is the canonical 根系 of $\mathfrak{g}$ and that $B(\mathfrak{g})$ is its 標準基底. 群 Aut($\mathfrak{g}$) operates on $\mathfrak{h}(\mathfrak{g})$ leaving $R(\mathfrak{g})$ and $B(\mathfrak{g})$ stable; 元 of Aut($\mathfrak{g}$) that operate trivially on $\mathfrak{h}(\mathfrak{g})$ are those of Aut$_0(\mathfrak{g})$.

#### 命題 6 {#lie-viii-s5-prop-6 .statement tag=0121}

$\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数とします。 We have, with 記法 in no. 1, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Ker $\varepsilon =$ Aut$_e(\mathfrak{g}).f(T_Q)$.

By §3, no. 3, Cor. of Prop. 10, Aut$_0(\mathfrak{g}) =$ Aut$_e(\mathfrak{g})$.Aut$_0(\mathfrak{g},\mathfrak{h})$. On the other hand, $\varepsilon$(Aut$_e(\mathfrak{g},\mathfrak{h})$)$\supset W(R)$ by §2, no. 2, Cor. Thの。 2、つまり、Aut$_0(\mathfrak{g},\mathfrak{h}) =$ Aut$_e(\mathfrak{g},\mathfrak{h})$.Ker$\varepsilon$。

#### 注意 3 {#lie-viii-s5-n3-rem-3 .statement tag=0122}

提案 6 は、標準準同型を示しています。

$\iota : T_Q/$Im(T$_P$)$\rightarrow$ Aut$_0(\mathfrak{g})/$Aut$_e(\mathfrak{g})$,

no. 2 の図式によって引き起こされたものは全射的です。 In particular, Aut$_e(\mathfrak{g})$ 含む導来群 of Aut$_0(\mathfrak{g})$; we shall see (§11, no. 2, Prop. 3) that they are actually equal. Moreover, it can be shown that $\iota$ is injective, in other 語 that $f(T_Q)\cap$ Aut$_e(\mathfrak{g}) =f'(T_P)$,

(cf. §7、演習$26d$)$)$。

#### 命題 7 {#lie-viii-s5-prop-7 .statement tag=0123}

$\mathfrak{g}$ を、$\mathfrak{g}$ の分割可能な半単純リー代数、$\mathfrak{b}$ ボレル部分代数、および $\mathfrak{g}$ 含む $\mathfrak{b}$ の$\mathfrak{p}_1$ と $\mathfrak{p}_2$ の別個の放物線部分代数とします。 Then $\mathfrak{p}_1$ and $\mathfrak{p}_2$ are not 共役 under Aut$_0(\mathfrak{g})$.

$k$ は代数的に閉じていると仮定できます。 $s\in$ Aut$_0(\mathfrak{g})$ が $s(\mathfrak{p}_1) =\mathfrak{p}_2$ となるようにします。 $\mathfrak{h}$ を、$\mathfrak{b}\cap s(\mathfrak{b}) ($§3, no. 3 に含まれる$\mathfrak{g}$ のカルタン部分代数とする、提案 10)。 $\mathfrak{h}$と$s(\mathfrak{h})$は$s(\mathfrak{b})$のカルタン部分代数なので、$e^{adu}(\mathfrak{h}) =s(\mathfrak{h})$となるような$u\in [\mathfrak{b},\mathfrak{b}]$が存在します（第3章VII, §3, no. 4）。 置き換えること $s$ $e^{-adu}s$ により、$s(\mathfrak{h}) =\mathfrak{h}$、$s$、そして誘導するが$\mathfrak{h}$ 元 $\sigma$ の Weyl 群 W の場合に帰着します。 $(\mathfrak{g},\mathfrak{h})$ (提案 4)。 Cをワイル室対応するから$\mathfrak{b}$とします。次に、$\mathfrak{p}_1$ と $\mathfrak{p}_2$ 対応するは、C のクロージャに含まれる $\mathfrak{h}_{\mathbf{R}}$ のファセット $F_1$ と $F_2$ になります。 $\sigma (F_1) = F_2$があります。 $\sigma \in W$ なので、これは $F_1= F_2$ (第 2 章 V, §3, no. 3) であるため、$\mathfrak{p}_1=\mathfrak{p}_2$ を意味します。

#### 注意 4 {#lie-viii-s5-n3-rem-4 .statement tag=0124}

$\mathfrak{g}$ を、Aut$_0(\mathfrak{g})$ が作用する $\mathfrak{g}$、集合の放物線部分代数の分割可能な半単純リー代数、$\mathscr{P}$ 集合とします。 注意の記法を保持します。 2. $\Sigma$ を $B(\mathfrak{g})$ の部分集合とします。 $\Sigma$ を与えることは、B のすべての $x= (\mathfrak{h},B)\in X$、部分集合 $\Sigma_x$ に対して与えることと同等であり、$s_{x',x}$ は、任意の $x, x'\in X$ に対して $\Sigma_x$ から $\Sigma_{x'}$ かかります。 $\mathfrak{p}_x$ を $\mathfrak{g}$ 対応するから $\Sigma_x$ までの放物線部分代数とします (§3, no. 4, 注意)。 Aut$_0(\mathfrak{g})$ の $\mathfrak{p}_x$ の軌道は、$x'\in X$ では $\mathfrak{p}_{x'}$ の集合です。これは、$\mathfrak{P}(B(\mathfrak{g}))$から$\mathscr{P}/$Aut$_0(\mathfrak{g})$までの定義する写像です。この写像は、§3, no. 4の注意によって全射的であり、提案7によって単射的です。

### 4. ザリスキー 位相オン オータム($\mathfrak{g}$)

#### 命題 8 {#lie-viii-s5-prop-8 .statement tag=0125}

V を自己準同型のベクトル空間 $\mathfrak{g}$ の集合とします。その後、Aut($\mathfrak{g}$)はVでザリスキー位相に向けてクローズされます(章VII、アプリI)。

K を $\mathfrak{g}$ の殺害形とします。 $s\in$ Aut($\mathfrak{g}$) の場合、

$$
[sx, sy] = [x, y] \tag{2}
$$

$$
K(sx, sy) = K(x, y) \tag{3}
$$

すべての$x, y\in \mathfrak{g}$に。逆に、$s$ をすべての $x, y\in \mathfrak{g}$ に対して V 満たす (2) と (3) の元とします。すると、Ker($s$) $= 0$ なので、$s$ は全単射で、$s\in$ Aut($\mathfrak{g}$) となります。ただし、V から $\mathfrak{g}$ および $k$ までのすべての $x, y\in \mathfrak{g}$、写像、$s \rightarrow [sx, sy]$、$s \rightarrow K(sx, sy)$ は多項式です。

#### 命題 9 {#lie-viii-s5-prop-9 .statement tag=0126}

$\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数とします。

(i) 群 $f(T_Q)$ は、ザリスキー 位相の 8 月 ($\mathfrak{g}$) に休業となります。

(ii) 群 $f(q(T_P))$ はザリスキー位相の$f(T_Q)$ に密集しています。

主張 (i) は、等式 $f(T_Q) =$ Aut($\mathfrak{g},\mathfrak{h}$)$\cap$Ker$\varepsilon$ (提案 2) から続きます。 $m= (P(R) : Q(R))$を入れます。 F を V で多項式関数とします。 F は $f(T_Q)$ の元ごとの $m$ 番目の冪に消えると仮定し、$F|f(T_Q) = 0$ であることを示します。 補題 3 を考慮すると、これは (ii) を証明します。

$\mathfrak{h}$ に同一性を誘導し、それぞれの $\mathfrak{g}^{\alpha}$ 安定を残す集合 V の元の $V'$ は、$k^R$ で識別できます。 $F'$ を F から $V'=k^R$ の制限とします。 多項式関数です。 $f(T_Q)\subset V'$ があります。 $B = (\alpha_1, . . . , \alpha_l)$ を R の基底とします。すべての $t= (t_1, . . . , t_l)\in k^{*B}$ について、$\varphi (t)$ を Q(R) から群 $k^*$ の拡大する $t$ までの準同型とします。すると、$F'(f(\varphi (t)))$ は有限の和として書くことができます。

$$
\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{n_1}_1. . . t^{n_l}_l= H(t_1, . . . , t_l)
$$

仮定までに、

$$
0 = H(t^m_1, . . . , t^m_l) =\sum_{n_1,...,n_l\in\mathbf{Z}}c_{n_1,...,n_l}t^{mn_1}_1. . . t^{mn_l}_l
$$

$t_1, . . . , t_l\in k^*$ 全員のために。したがって、$c_{n_1,...,n_l}$ は、$k^{*l}$ で消える$l$ 変数の多項式の係数です。したがって、それらはすべて零です。

#### 命題 10 {#lie-viii-s5-prop-10 .statement tag=0127}

$\mathfrak{g}$ は分割可能であると仮定します。

(i) 群 Aut$_e(\mathfrak{g})$ は、ザリスキー位相の Aut$_0(\mathfrak{g})$ に密集しています。

(ii) 群 Aut$_e(\mathfrak{g})$ と Aut$_0(\mathfrak{g})$ はザリスキー 位相で接続されています。

提案$3,f(q(T_P))\subset$ Aut$_e(\mathfrak{g})$ による。すべての $s\in$ Aut$_e(\mathfrak{g})$ について、提案 9 によるザリスキー 位相含む $s.f(T_Q)$ の $s.f(q(T_P))$ の閉鎖。 したがって、Aut$_e(\mathfrak{g})$ 含む Aut$_e(\mathfrak{g}).f(T_Q) =$ の閉鎖Aut$_0(\mathfrak{g})$ (提案 6)。これは(i)を証明します。

Aut$_e(\mathfrak{g}) =\Omega \cup \Omega '$を、ザリスキー位相の比較的オープンな部分集合と$\Omega \not=\emptyset$によって形成されたAut$_e(\mathfrak{g})$の分割とします。 $\omega \in \Omega$ で、$x$ が $\mathfrak{g}$ の冪零元である場合、$k$ から Aut$_e(\mathfrak{g})$ までの写像 $\tau :t \rightarrow \omega$ exp($t$ ad $x$) は多項式であるため、ザリスキーでは連続です。 位相;その結果、$\tau (k)$ が接続されます。 $\omega \in \tau (k)$ から、$\tau (k)\subset \Omega$ になります。従って、$\Omega$.(exp ad $kx$)$\subset \Omega$、つまり $\Omega$.Aut$_e(\mathfrak{g})\subset \Omega$ および $\Omega =$ Aut$_e(\mathfrak{g})$ となります。これは、Aut$_e(\mathfrak{g})$ が接続されていることを証明します。 (i) により、Aut$_0(\mathfrak{g})$ が接続されることになります。 Q.E.D.

Aut$_0(\mathfrak{g})$がザリスキー位相のVで閉じられており、Aut($\mathfrak{g}$)の単位元の接続された成分であることがわかります(§8, no. 4、提案6の修正)。一方、Aut$_e(\mathfrak{g})$は、ザリスキー位相では一般的に閉鎖されません。

\*$(\mathfrak{g},\mathfrak{h})$ が分裂であると仮定します。 群 Aut$_0(\mathfrak{g})$ は、自明中心 (随伴群) と接続された半単純代数群 G の $k$ 点の群 $G(k)$ です。 群 $f(T_Q)$ は $H(k)$ に等しく、ここで H はリー代数 $\mathfrak{h}$ を持つ G のカルタン部分群です。 G の普遍的カバー (代数的な意味で) $\widetilde{G}$ における H の逆像 $\widetilde{H}$ は、$k$ 点の群として $T_P$ を持ちます。 $G(k) =$ Aut$_0(\mathfrak{g})$ の $\widetilde{G}(k)$ の像は群 Aut$_e(\mathfrak{g})$ です。\*

### 5. リー群ケース

#### 命題 11 {#lie-viii-s5-prop-11 .statement tag=0128}

$k$ が $\mathbf{R},\mathbf{C}$ または非離散完全ウルトラメトリック体であると仮定します。 $\mathfrak{h}$ を $\mathfrak{g}$ の分裂カルタン部分代数とします。

(i) Aut($\mathfrak{g},\mathfrak{h}$) は、リー代数 ad$\mathfrak{h}$ を含む Aut($\mathfrak{g}$) の嘘部分群です。

(ii) $f(T_Q)$ と $(q\circ f)(T_P)$ は Aut($\mathfrak{g},\mathfrak{h}$) の部分群が開いています。

(iii) Aut$_e(\mathfrak{g})$ は Aut($\mathfrak{g}$) のオープン部分群です。

(iv) $k=\mathbf{R}$ または $\mathbf{C}$ の場合、Aut$_e(\mathfrak{g})$ は、他の語 Int($\mathfrak{g}$) における Aut($\mathfrak{g}$) の同一性成分です。

章著。 III, §3, no. 8、コル。提案29の2、および提案36のno. 10、Aut($\mathfrak{g},\mathfrak{h}$)はAut($\mathfrak{g}$)の嘘部分群で、そのリー代数は広告$x(x\in \mathfrak{g})$の集合であり、その他では(広告$x$)$\mathfrak{h}\subset \mathfrak{h}$となる。 語広告$\mathfrak{h}$。

$H\in \mathfrak{h}$ にしましょう。次のプロパティを持つ $\varepsilon  >0$ が存在します: $t\in k$ と $|t|< \varepsilon$ の場合、exp($t\gamma (H)$) はすべての $\gamma \in P(R)$ に対して定義され、写像 $\gamma  \rightarrow$ exp($t\gamma (H)$) は P(R) から準同型 $\sigma_t$ です。 $k^*$。 $|t|< \varepsilon$ については、exp($t$ ad H) が定義され、$\mathfrak{h}$ の恒等度誘導すると$\mathfrak{g}^{\alpha}$ ホモテティー の誘導するが比 $\sigma_t(\alpha )$ で定義されます。従って、exp $t$ ad $H\in (q\circ f)(T_P)$。これは、(i) を考慮すると、Aut($\mathfrak{g},\mathfrak{h}$) の 1 の $(q\circ f)(T_P)$ 含む近傍が証明され、その結果、Aut($\mathfrak{g},\mathfrak{h}$) のオープン部分群になります。 なおさら$,f(T_Q)$はAut($\mathfrak{g},\mathfrak{h}$)のオープン部分群です。

すべての $\alpha \in R$、exp ad $\mathfrak{g}^{\alpha}\subset$ Aut$_e(\mathfrak{g})$。 (ii) を考慮すると、Aut($\mathfrak{g}$) の 1 の Aut$_e(\mathfrak{g})$ 含む近傍となり、(iii) が証明されます。

$k=\mathbf{R}$ または $\mathbf{C}$ と仮定します。すると、Aut$_e(\mathfrak{g})$はAut($\mathfrak{g}$)の同一性成分Cに含まれ(VII, §3, no. 1章)、(iii)によりAut($\mathfrak{g}$)に開かれる。従って、Aut$_e(\mathfrak{g}) = C$。最後に、第 4 章による C = Int($\mathfrak{g}$) です。 III, §9, no. 8、提案 30 (i)。

### 練習問題 {#lie-viii-s5-exercises}

[§ 5 に対して練習問題](exercises/s5/)を参照してください。
