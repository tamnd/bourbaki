---
book: int
book_title: Integration
chapter: IX
chapter_title: MEASURES ON HAUSDORFF TOPOLOGICAL SPACES
section: 3
section_title: Measures and additive set functions
lang: ja
source: int-vii-ix
book_pages: INT IX.41-INT IX.49, INT IX.108-INT IX.112
pdf_pages: 0223-0231, 0290-0294
extraction: ocr
subsections:
    - "no": 1
      title: Measures and additive set functions of compact sets
      page: 41
      pdf_page: 223
    - "no": 2
      title: Inner regular set functions
      page: 44
      pdf_page: 226
    - "no": 3
      title: Radon spaces
      page: 46
      pdf_page: 228
statements: 17
exercises: 18
content_sha256: e7f93e8e75db9a43d8fe3379c2790e8e716835e762e8480be166910d4b0e060c
translated_from: content/en/int/IX/03_s3_measures_and_additive_set_functions.md
translation_method: google
source_content_sha256: b7143e1dccb4a50f4c6430b942b6320cab29a534320ec6405180a553d32e45d9
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-dda8bbaf
glossary_version: 34
glossary_terms_sha256: 9c9c3e7060c20178c023d83f51143cf4f38693782bcfe7919b72dff7dd157115
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## § 3。対策と加法的集合写像

この切断では、ハウスドルフ位相幾何学空間 T のコンパクト部分集合と T のボレル部族の集合を、それぞれ $\mathscr{K}(T)$ と $\mathscr{B}(T)$ で表すことにします。

### 1. コンパクト集合の対策と加法的集合写像

#### 定理 1 {#int-ix-s3-thm-1 .statement tag=09PN}

— T をトポロジー 空間、および $\mathscr{K}(T)$ から $\mathbf{R}_+$ への I 写像とする。 位数では、すべての $K \in \mathscr{K}(T)$ に対して $I(K) = \mu^\bullet(K)$ となるような尺度 $\mu$ が T に存在するため、次の条件が I 満たすとなることが必要かつ十分です。

1) K と L が $K \subset L$ となるような T のコンパクト部分集合である場合、$I(K) \leq I(L)$ (「I は増加する」)。

2) K と L が T の部分集合よりコンパクトな場合、$I(K \cup L) \leq I(K) + I(L)$。

3) K と L が T の互いに素コンパクト部分集合である場合、$I(K \cup L) = I(K) + I(L)$ (「I は加法的」)。

4) T のコンパクト部分集合のすべての減少する有向族 $(K_\alpha)_{\alpha \in A}$ に対して、1 つは $I(\bigcap_{\alpha \in A} K_\alpha) = \inf_{\alpha \in A} I(K_\alpha)$ を持ちます。

5) すべての $x \in T$ に対して、次のような x の近傍 V が存在します。
$$
\sup_{\substack{K \in \mathscr{K}(T) \\ K \subset V}} I(K) < +\infty
$$
(「I はローカルに限定されています」)。

したがって、メジャー $\mu$ は一意になります。

The uniqueness of $\mu$ follows from the Cor. of Prop. 2 of § 1, No. 2. 上記の条件は必要で、最初の 3 つは明らかな方法で、最後の 1 つは $\mu^\bullet$ が局所的に制限された制約であるという事実から、そして条件 4) は Cor によるものです。 § 1, No. 6の提案5の。

これら条件が十分であることを示すために、T がコンパクトである場合を扱うことから始めます。

#### 補題 1 {#int-ix-s3-lem-1 .statement tag=09PO}

T がコンパクトであり、集合 l = I(T) であると仮定します。 $A \subset T$、集合ごとに

$$
J(A) = \sup_{\substack{K \in \mathscr{K}(T) \\ K \subset A}} I(K)
$$

そして、$\Phi$ を $A \subset T$ の集合とし、$J(A) + J(\mathbf{C}A) = l$ とします。 集合 $\Phi$ は、含む $\mathscr{K}(T)$ と$\Phi$ の写像 $J$ が増加するとなるクランです。

$J$ は $I$ を延長して増加する集合写像となり、$A \subset T$ ごとに $J(A) + J(\mathbf{C}A) \leq l$ になることは明らかです。

$K$ と $S$ を、$T$ の 2 つのコンパクトな集合とします。まずそれを示します

$$
J(K \cap S) + J(\mathbf{C}K \cap S) = J(S).
$$

$I$から$\mathscr{K}(S)$の制限と、$J$から$\mathfrak{P}(S)$の制限を考えると、$S = T$の場合にはすぐに簡約するが1つ出ます。 $T$ が正常であるため、$K$ はそのコンパクトな近傍の減少するの有向族の共通部分であり、条件 4) は、$\varepsilon > 0$ ごとに、$I(H) \leq I(K) + \varepsilon$ となるような $K$ のコンパクトな近傍 $H$ の存在を暗示します。 $L$ を $T - H$ の閉包とします。 $L$ はコンパクト、$L \cap K = \varnothing$ と $H \cup L = T$、したがって $l = I(H \cup L) \leq I(H) + I(L) \leq I(K) + I(L) + \varepsilon$ (条件 2))、よって関係 $J(K) + J(\mathbf{C}K) \geq I(K) + I(L) \geq l - \varepsilon$。 $\varepsilon$は任意なので$J(K) + J(\mathbf{C}K) = l$。 これは公式 (2) と包含 $\mathscr{K}(T) \subset \Phi$ を証明します。

ここで、$\Phi$ がクランであることを証明してみましょう。 $\Phi$ は補体への移行下では明らかに安定しているため、$A_1$ と $A_2$ が $\Phi$ の元を表す場合、$A_1 \cup A_2 \in \Phi$、または再度以下を示すだけで十分です。

$$
J(A_1 \cup A_2) + J(\mathbf{C}(A_1 \cup A_2)) \geq l.
$$

$\varepsilon$ 数 $> 0$ で表し、$i = 1, 2$ について、$K_i$ を $A_i$ に含まれるコンパクト集合と、$L_i$ を $\mathbf{C}A_i$ に含まれるコンパクト集合とします。

$$
I(K_i) \geq J(A_i) - \varepsilon, \quad I(L_i) \geq J(\mathbf{C}A_i) - \varepsilon.
$$

集合 $M_1 = K_1 \cup L_1$; 関係 $l = J(M_1) + J(\mathbf{C}M_1)$ と

$$
J(M_1) = I(K_1) + I(L_1) \geq J(A_1) + J(\mathbf{C}A_1) - 2\varepsilon = l - 2\varepsilon
$$

$J(\mathbf{C}M_1) \leq 2\varepsilon$ を暗示します。次に、$S$ が $T$ の圧縮部分集合である場合、関係 (2) ($K = M_1$ に適用) は、$J(S) \leq J(M_1 \cap S) + 2\varepsilon$、よってを意味します。

$$
J(S) \leq J(K_1 \cap S) + J(L_1 \cap S) + 2\varepsilon.
$$

$S = K_2$ と $S = L_2$ を作成することで得られる不等式を追加し、不等式 $J(K_2) + J(L_2) \geq l - 2\varepsilon$ と、$K_1 \cap K_2$、$L_1 \cap K_2$、$K_1 \cap L_2$ が 3 つの互いに素がコンパクトな集合に含まれるという事実を考慮してみましょう。 $A_1 \cup A_2$。これら 3 つのコンパクト集合のうち $C$ 和集合で表すと、次のようになります。

$$
l - 2\varepsilon \leq J(K_2) + J(L_2) \leq J(C) + J(L_1 \cap L_2) + 4\varepsilon \\
\leq J(A_1 \cup A_2) + J(\mathscr{C}(A_1 \cup A_2)) + 4\varepsilon,
$$

よっては、$\varepsilon$ の恣意性を考慮して、すぐに望ましい公式 (3) になります。これが確立されたので、前述の不等式は $J(C) \geq J(A_1 \cup A_2) - 6\varepsilon$ を意味します。 $A_1$ と $A_2$ が互いに素である場合、$C$ は $K_1 \cap L_2 \subset A_1$ と $K_2 \cap L_1 \subset A_2$ の和集合であり、そこから $J(A_1 \cup A_2) \leq J(A_1) + J(A_2)$ が推測されます。逆の不等式は明白であり、$J$は確かに$\Phi$に加算され、補題が確立されます。

$T$がコンパクトな場合の定理の証明を完成させましょう。 $\mathscr{E}(\Phi)$ を、一様収束の位相を備えた $T$ の $\Phi$ ステップ写像のベクトル空間とします (Ch. IV, §4, No. 9、定義 4)。 加法的関数 $J$ に関連する $\mathscr{E}(\Phi)$ 上の正の線型形式を再び $J$ で表すことにします (上記、提案 18)。 $J(T) = l$ なので、$J$ は連続で、ノルム $l$ になります。次に、$\mathscr{H}$ を一様収束の位相に対する $\mathscr{E}(\Phi)$ の閉包とします。 $J$ が連続性によって$\mathscr{H}$ の *正の* 線型形式まで拡張される可能性があることがすぐに検証され、再び $J$ で示されます。 $\mathscr{H}$ 含む $\mathscr{C}(T)$ (引用文献、No. 10、提案 19) から、$J$ から $\mathscr{C}(T)$ までの制限は、$\mu$ の肯定的な尺度です。 $T$ の各コンパクト部分集合 $K$ に対して $\mu^\bullet(K) = I(K)$ であることを示すことが残っています。ここで、$\mu^\bullet(K) = \inf_{f \in S_K} \mu^\bullet(f)$ があります。ここで、$S_K$ は、$\mathscr{C}(T)$ の元のうち集合 、すなわち $\geq \varphi_K$ を表します (§ 1, No. 6、提案 5)。 $f \in \mathscr{C}(T)$ は $J(f) = \mu^\bullet(f)$ なので、明らかに $J(K) \geq \inf_{f \in S_K} J(f)$ であることが示されれば十分です。 補題 1 の証明のように、$H$ を $J(H) \leq J(K) + \varepsilon$ となるような $K$ のコンパクトな近傍とし、$f$ を 0 と 1 の間で、$K$ で 1 に等しい、$T$ 上で連続する写像とする。 $H$ 外側 0 (GT、IX, §4, No. 1、提案 1)。それから

$$
J(f) \leq J(H) \leq J(K) + \varepsilon;
$$

$\varepsilon$ が任意であるため、望ましい不等式が証明され、$T$ がコンパクトな場合、定理が確立されます。

次に、一般的なケースに移りましょう。 $T$ のすべてのコンパクト集合 $L$ について、$I_L$ を $I$ ～ $\mathfrak{K}(L)$ の制限とします。たった今扱った特殊なケースでは、すべてのコンパクト集合 $K \subset L$ に対して $\mu_L(K) = I_L(K)$ というような、$L$ に一意のメジャー $\mu_L$ が存在します。次に、$L'$ を $L$ に含まれる圧縮集合とします。すべてのコンパクト集合 $K \subset L'$ には $(\mu_L)_{L'}^\bullet(K) = \mu_{L'}^\bullet(K) = \mu_{L'}^\bullet(K)$ があるため、$\mu_{L'} = (\mu_L)_{L'}$ になります。 写像 $\mu : L \mapsto \mu_L$ は事前対策です。 条件 5) は、$\mu$ がメジャーであり、すべてのコンパクトな $K \subset T$ に対して関係 $I(K) = \mu^*(K)$ が明らかであることを表します。

#### 注意 1 {#int-ix-s3-n1-rem-1 .statement tag=09PP}

条件 4) は、定理 1 の主張で、次の条件 ('right-continuity') に置き換えることができます。
$4')$ すべての $K \in \mathscr{K}(T)$ とすべての $\varepsilon > 0$ に対して、オープン集合 $U$ 含む $K$ が存在し、すべてのコンパクト集合 $H \subset U$ に対して $I(H) \leq I(K) + \varepsilon$ が存在します。
なぜなら、$\mu$ が尺度である場合、写像 $I : K \mapsto \mu^*(K)$ は $4'$ を満たすからです (§ 1, No. 9、提案 13)。逆に、$I$ が 1) と $4'$ を満たすとします。 $I$ が 4) を満たすことを示しましょう。 定理 1 の主張のような記法、選ぶ $\varepsilon > 0$、およびオープン集合 $U$ 含むでは、コンパクトな集合 $K = \bigcap_{\alpha \in A} K_\alpha$ など $4'$) は次のようになります。満足です。したがって、$K_\beta \subset U$ となるような添字 $\beta \in A$ が存在し、これは次のことを意味します。
$$
\inf_{\alpha \in A} I(K_\alpha) \leq I(K_\beta) \leq I(K) + \varepsilon
$$
4) は実際に検証されています。

#### 注意 2 {#int-ix-s3-n1-rem-2 .statement tag=09PQ}

条件 2) および 3) の集合は、定理 1 の主張で、次の条件に置き換えることができます。
$K$ と $L$ が $T$ の部分集合よりコンパクトである場合、
$$
I(K \cup L) + I(K \cap L) = I(K) + I(L).
$$
確かに、この条件は 2) と 3) を意味しており、その一方で
$$
\mu^*(K \cup L) = \mu^*(K \cap L) = \mu^*(K) + \mu^*(L)
$$
すべてのメジャー $\mu$ について、特性写像の間の関係 $\varphi_{K \cup L} + \varphi_{K \cap L} = \varphi_K + \varphi_L$ によって。

### 2. 内部レギュラー 集合写像

#### 定義 1 {#int-ix-s3-def-1 .statement tag=09PR}

$T$ をトポロジー 空間とし、$\mathscr{B}(T)$ を $T$ のボレル部族とします。 $I$を$\mathscr{B}(T)$の写像を$\overline{\mathbf{R}}_+$にします。
a) $I$ は、$\mathscr{B}(T)$ のペアごとの互いに素元の各数列 $(A_n)$ に対して、
$$
I\left( \bigcup_n A_n \right) = \sum_n I(A_n).
$$
b) 集合 $A \in \mathscr{B}(T)$ ごとに、$I$ は内部正規であると言われます。
$$
I(A) = \sup_K I(K),
$$
ここで、$K$ は、$A$ のコンパクトな部分集合の集合を上回ります。

c) I は、$I(T) < +\infty$ が有界である (局所的に有界である) と言われます (それぞれの点 $x \in T$ が $I(V) < +\infty$ のようなオープン近傍 $V$ を認める場合)。

#### 注意 1 {#int-ix-s3-n2-rem-1 .statement tag=09PS}

条件 a) は、I が $\mathscr{B}(T)$ の増加する写像 (包含順) が $\overline{\mathbf{R}}_+$ に入るということを明らかに示しています。

#### 注意 2 {#int-ix-s3-n2-rem-2 .statement tag=09PT}

I が可算加算的であると仮定します。 $(A_n)_{n \in \mathbf{N}}$ をボレル集合の増加する数列とし、$A = \bigcup_{n \in \mathbf{N}} A_n$ とします。 集合 $D_0 = A_0$、$D_n = A_n - A_{n-1}$ は互いに素のペアであり、それらの和集合は A なので、$I(A) = \sum_n I(D_n) = \lim_{n \to \infty} I(A_n)$ になります。同様に、$(B_n)$ がボレル集合の減少列で、$I(B_0) < +\infty$ の場合、$I(\bigcap_n B_n) = \lim_{n \to \infty} I(B_n)$: 上記を集合 $A_n = B_0 - B_n$ に適用すれば十分です。

#### 注意 3 {#int-ix-s3-n2-rem-3 .statement tag=09PU}

$(A_n)$ を T の Borel 集合の任意の数列とします。I が可算加法である場合、$I(\bigcup_n A_n) \leq \sum_n I(A_n)$ になります。前の注意により、有限列に対してこの不等式を確立するだけで十分です。 1 つはすぐに簡約する 、2 つの場合は集合 $A_1$ と $A_2$ です。しかし、関係 (4) は次のことを意味します。

$$
I(A_1 \cup A_2) = I(A_1) + I(A_2 - (A_1 \cap A_2)) \leq I(A_1) + I(A_2).
$$

目的の不等式がすぐに続きます。

#### 注意 4 {#int-ix-s3-n2-rem-4 .statement tag=09PV}

I が可算加法であり、局所的に有界な写像である場合、先行する注意は、すべてのコンパクト集合 $K \subset T$ に対して $I(K) < +\infty$ を即座に意味します。

#### 注意 5 {#int-ix-s3-n2-rem-5 .statement tag=09PW}

I が加法的である場合、つまり有限列について (4) を満たす場合、および I が内部正則である場合、I は可算加法的であることを示すことができます (Exer. 7)。読者は、Th の証明で加法性と内部規則性のみが使用されていることも確認できます。以下2。

#### 定理 2 {#int-ix-s3-thm-2 .statement tag=09PX}

— T をトポロジー 空間とし、I を $\mathscr{B}(T)$ で定義され、$\overline{\mathbf{R}}_+$ に値が含まれる写像とします。 位数では、すべての $A \in \mathscr{B}(T)$ に対して $\mu^*(A) = I(A)$ となるような測度 $\mu$ が T に存在するということは、I が可算加算的であり、局所有界であり、内部正則であることが必要かつ十分です。したがって、メジャー $\mu$ は一意になります。

これら 3 つの条件が必要です。なぜなら、$\mathscr{B}(T)$ 上の写像 $A \mapsto \mu^*(A)$ は可算加算的 (§ 1, No. 5、提案 4 の補正)、局所的に定義の尺度によって制限され (§ 1, No. 2、定義 5)、そして内部の注意 3 によって正則だからです。 § 1, No. 2。

私たちは存在に移ります。 Iから$\mathscr{K}(T)$の制限はThの主張の条件1)、2)、3)、5)を満たすことが明らかです。 1; 4) も満たされることを示しましょう。 K を T のコンパクト部分集合、コンパクト集合の減少する有向族 $(K_\alpha)_{\alpha \in A}$ の共通部分、そして $\varepsilon$ を数 $> 0$ とします。 I は局所的に限定されており、$I(V) < +\infty$ のような K の開いた (したがって Borel) 近傍 V が存在し、その後、$K_\alpha \subset V$ のような添字 $\alpha$ が存在します。必要に応じて記法を変更すると、すべての $\alpha \in A$ に対して $K_\alpha \subset V$ と仮定できます。 Iの内部規則性により、$I(L) \geq I(V - K) - \varepsilon$となるようなコンパクトな集合$L \subset V - K$が存在します。 L は K と交わらないので、$L \cap K_\alpha = \varnothing$ となるような添字 $\alpha$ が存在し、その場合、$I(V - K_\alpha) \geq I(L) \geq I(V - K) - \varepsilon$ になります。 $K_\alpha \subset V$ なので、$I(K_\alpha) \leq I(K) + \varepsilon$ と条件 4) が検証されることになります。

Thさんより1、すべての $K \in \mathscr{K}(T)$ に対して $\mu^\bullet(K) = I(K)$ となるような尺度 $\mu$ が存在します。 $\mathscr{B}(T)$ における集合写像 $\mu^\bullet$ と $I$ の内部の規則性は、すべての $A \in \mathscr{B}(T)$ について $\mu^\bullet(A) = I(A)$ であることを意味し、存在が証明されます。 $\mu$の一意性はThの一意性主張から続きます。 1.

### 3. ラドン空間

#### 定義 2 {#int-ix-s3-def-2 .statement tag=09PY}

*T を位相ベクトル空間とします。 One says that T is a Radon (resp. strongly Radon) space if T is Hausdorff and if every function defined on the Borel tribe $\mathscr{B}(T)$ of T, with values in $\overline{\mathbf{R}}_+$, that is countably additive and bounded (resp. locally bounded) is inner regular.*

たとえば、すべてのポーランド語空間は強力にラドンであることは後でわかります (提案 3)。特に、可算な基底を持つ局所的にコンパクトな空間はすべて強くラドンです。

強いラドンではないラドン空間も存在します。

#### 命題 1 {#int-ix-s3-prop-1 .statement tag=09PZ}

*すべてのリンデロフ*$^{(1)}$* ラドン空間は強いラドンです。*

T をラドンであるリンデロフ空間とし、I を部族 $\mathscr{B}(T)$ 上の集合写像とします。これは正で可算加算的で局所的に有界です。 $I(V) < +\infty$ 形が T のカバーとなるようなオープン集合 V から、可算カバー $(V_n)_{n \in \mathbf{N}}$ を抽出できます。 $n \in \mathbf{N}$ ごとに集合 $G_n = V_0 \cup V_1 \cup \cdots \cup V_n$; $n \geq 1$ の場合は集合 $H_0 = G_0$ と $H_n = G_n - G_{n-1}$。最後に、$\mathscr{B}(T)$ 上の $I_n$ 集合写像 $A \mapsto I(A \cap H_n)$ で表します。これは明らかに可算加算的であり、有界です。 T の集合 $H_n$ 形分割なので、$I = \sum_n I_n$ になります。 空間 T はラドンであり、$n \in \mathbf{N}$ ごとに、すべての $A \in \mathscr{B}(T)$ に対して $\mu_n^\bullet(A) = I_n(A)$ となるような、T 上の制限された尺度 $\mu_n$ が存在します。したがって、$\sum_n \mu_n^\bullet(A) = I(A)$ も同様です。 I は局所的に有界であるため、ファミリー $(\mu_n)$ は合計可能です (§ 1, No. 7、提案 7)。 $\mu$ が $\sum_n \mu_n$ を表す場合、すべての $A \in \mathscr{B}(T)$ に対して $\mu^\bullet(A) = I(A)$ が得られ、I が正規の内部であることがわかります。他の語では、T は強くラドンです。

トポロジカル空間 T の部分集合 A は、A が T 上のすべてのメジャー $\mu$ について $\mu$ 測定可能である場合、*普遍的に測定可能* であると言われることを思い出してください。これは、*コンパクト サポート* を使用して、A が T 上のすべてのメジャー $\mu$ について $\mu$ 測定可能であるというというと同等です。 (§ 1, No. 8、提案9)。

(1) (GT, I, §9, Exer. 14; TG, IX, 付録 I) を思い出してください。*Lindelöf 空間* は位相的空間 T であり、T 含むのすべての開いた被覆は可算被覆になります。

#### 命題 2 {#int-ix-s3-prop-2 .statement tag=09Q0}

— X をトポロジー 空間および X の T 部分空間とします。

a) T がラドン空間であると仮定します。次に、$\mathscr{B}(X)$ で定義された、正で可算加算的で有界であるすべての写像 I について、

$$
\sup_{\substack{K \text{ compact} \\ K \subset T}} I(K) = \inf_{\substack{B \in \mathscr{B}(X) \\ B \supset T}} I(B).
$$

さらに、T はX で普遍的に測定可能です。

b) 逆に、X がラドン空間であり、T が X で普遍的に測定可能であると仮定します。その場合、T はラドン空間です。

a)を証明しましょう。 (6) の右辺を $\alpha$ で示します。すべての $n \in \mathbf{N}$ に対して、$I(C_n) \leq \alpha + 2^{-n}$ となる集合 $C_n \in \mathscr{B}(X)$ 含む T が存在します。 設定 $C = \bigcap_n C_n$ の場合は、$T \subset C$、$I(C) = \alpha$ になります。 $A \in \mathscr{B}(T)$ の場合、$A = B \cap T$ (GT, IX, §6, No. 3) と集合 $J(A) = I(B \cap C)$ となるように、X の Borel 集合 B を選ぶとしましょう。この数は B の選択には依存しません。なぜなら、$B'$ が $A = B' \cap T$ となるような X の 2 番目のボレル集合である場合、$B \cap C$ と $B' \cap C$ は、B に含まれるボレル集合 M だけが異なります。 $C - T$、および$I(M) = 0$、Cの構成による。明らかに、すべてのコンパクト集合 $K \subset T$ に対して $J(K) = I(K)$ です。 $(A_n)$ を T の Borel 集合の数列とし、ペアごとに互いに素とし、それぞれの $n$ について、$B_n$ を $B_n \cap T = A_n$ となるような X の Borel 集合とします。必要に応じて、置き換えること $B_n$ $B_n - \left( \bigcup_{k < n} B_k \right)$ により、集合 $B_n$ がペアごとに互いに素であると仮定できます。 集合 $A = \bigcup_n A_n$ と $B = \bigcup_n B_n$;それから

$$
J(A) = I(B \cap C) = \sum_n I(B_n \cap C) = \sum_n J(A_n);
$$

従って、J は可算加法であり、写像が $\mathscr{B}(T)$ に限定されます。 T は仮定ラドン空間であるため、T には、$A \in \mathscr{B}(T)$ ごとに $J(A) = \mu^\bullet(A)$ となるような制限された尺度 $\mu$ が存在します。従って

$$
\alpha = J(T) = \mu^\bullet(T) = \sup_K \mu^\bullet(K) = \sup_K J(K),
$$

$\mu^\bullet$の定義による。従って、公式 (6) が成立します。

ここで、T が普遍的に測定可能であることを示しましょう。 $\lambda$ を X での制限された尺度とします。前の引数は $\mathscr{B}(X)$ の集合写像 $I : A \mapsto \lambda^\bullet(A)$ に適用できるため、次のような T のコンパクト部分集合の数列 $(K_n)$ が存在します (上記の記法を使用)

$$
\sup_n \lambda^\bullet(K_n) = J(T) = \lambda^\bullet(C).
$$

集合 $K' = \bigcup_{n \in \mathbf{N}} K_n$; $K'$ は $X$、$K' \subset T \subset C$、$\lambda^*(K') = \lambda^*(C)$ のボレルであるため、これら 3 つの集合の違いは $\lambda$ で無視できる程度の集合だけであるため、$T$ は $\lambda$ で測定可能です。これでa)の証明は完了です。

b)に移りましょう。 $X$ がラドン空間であり、$T$ が$X$ で普遍的に測定可能であると仮定します。 $I$ を、可算加法で有界である $\mathscr{B}(T)$ 上の正の写像とします。 $\mathscr{B}(X)$ 上の写像 $A \mapsto I(A \cap T)$ は正であり、可算加算的であり、有界であるため、すべての $A \in \mathscr{B}(X)$ に対して $I(A \cap T) = \nu^*(A)$ となるような、$X$ に有界測定$\nu$ が存在します。さて、$T$ は $\nu$ で測定可能です。前述の関係は、$T$ から互いに素である $X$ のすべてのコンパクト部分集合 $K$ について $\nu^*(K) = 0$ であることを示しているため、$\nu$ は $T$ に集中しています。従って、$X$ の各ボレル集合 $A$ に対して、$I(A \cap T) = \nu^*(A \cap T) = \mu^*(A \cap T)$ が得られます。ここで、$\mu$ は、$T$ で $\nu$ によって引き起こされる測度です。最後に、集合 $B \in \mathscr{B}(T)$ (GT、IX, §6, No. 3、*注意 2*) ごとに $I(B) = \mu^*(B)$ となり、$I$ は確かに内部正規です。

#### 系 {#int-ix-s3-n3-cor-1 .statement tag=09Q1}

— *$X$ がラドン空間である場合、$X$ のすべてのボレル部分集合 $T$ はラドンです。

なぜなら、$T$は普遍的に$X$で測定可能だからです。

#### 命題 3 {#int-ix-s3-prop-3 .statement tag=09Q2}

— *すべてのスーリン空間 (特にすべてのポーランド語またはルーシン空間) は強力なラドンです。*

$T$ をスーリン空間とします。 $T$ はリンデロフ空間 (TG、IX、付録 I、提案 1 の補正) であるため、(2) $T$ がラドン (提案 1) であることを示すだけで十分です。 $I$ を $\mathscr{B}(T)$ で定義された正の可算加算的で有界な写像とします。 $T$ の部分集合 $A$ ごとに、設定によって拡大する $I$ から $\mathscr{P}(T)$ まで、

$$
I(A) = \inf_{\substack{B \in \mathscr{B}(T) \\ B \supseteq A}} I(B).
$$

この拡大が $T$ (GT, IX, §6, No. 9) の *容量* であることを示しましょう。 関係 $A \subset A'$ が $I(A) \leq I(A')$ を暗示していることは明らかです。 $(A_n)$ を $T$ の部分集合の増加する数列とし、$A = \bigcup_n A_n$ とします。ボレル集合の集合、含む$A_n$が可算共通部分の間安定していると、各$n$には$A_n \subset B_n$と$I(A_n) = I(B_n)$のようなボレル集合$B_n$が存在します。 (提案 2 のcf. 証明)。 集合 $C_n = \bigcap_{p \geq n} B_p$; $C_n$ はボレル、$A_n \subset C_n \subset B_n$ なので $I(A_n) = I(C_n)$ です。一方、数列 $(C_n)$ は増加するです。 $C = \bigcup_n C_n$: 関係 $A \subset C$ が次のことを意味するとします。

$$
I(A) \leq I(C) = \lim_n I(C_n) = \lim_n I(A_n),
$$

(2) すべてのスースリン空間には、オープン集合 (GT、IX, §6, No. 2、提案 4) に対して可算な基底があり、したがってリンデロフ (GT、I, §9、Exer. 14) になります。

よって等式 $I(A) = \lim_n I(A_n)$ は明らかです。従って、I が容量となります。

$(H_n)$がTのクローズド集合の減少列であれば、明らかに$I\left( \bigcap_n H_n \right) = \inf_n I(H_n)$です。従って、T のすべてのスースリン部分集合 F は I に対応できるということになります (TG、IX, §6, No. 10、提案 15)。特に、T のすべての Borel 集合 A は容量可能です (*loc. cit.*, §6, No. 3, Prop. 10)。(3) 他の語では、

$$
I(A) = \sup_K I(K),
$$

ここで、K は A に含まれるコンパクト集合の集合を上回ります。 I が内部正規であることを証明しました。

#### 注意 {#int-ix-s3-n3-rem-1 .statement tag=09Q3}

— X をルーシン空間 (特にポーランド語空間) とし、(ルーシン) 正則空間 Y 上への X の全単射連続写像とする。(TG、IX, §6, No. 7、提案 14) 写像 $B \mapsto f^{-1}(B)$ は、X のボレル族に対する Y のボレル族の全単射です。 空間 X と Y はルーシンであるため、強力にラドンです (提案 3)。 写像 $\mu \mapsto f(\mu)$ は、Y の有界メジャーの集合上で、X の有界メジャーの集合の全単射であることがわかります。(4)

### 練習問題 {#int-ix-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
