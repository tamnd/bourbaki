---
book: alg
book_title: Algebra
chapter: II
chapter_title: LINEAR ALGEBRA
section: 8
section_title: Restriction of the field ofscalars in vector spaces
lang: ja
source: alg-i-iii
source_edition: 1998, Springer
book_pages: 317-325, 409-410
pdf_pages: 0341-0349, 0433-0434
extraction: ocr
subsections:
    - "no": 1
      title: DEFINITION OF K'-STRUCTURES
      page: 317
      pdf_page: 341
    - "no": 2
      title: Rationality for a subspace
      page: 318
      pdf_page: 342
    - "no": 3
      title: RATIONALITY FOR A LINEAR MAPPING
      page: 319
      pdf_page: 343
    - "no": 4
      title: RATIONAL LINEAR FORMS
      page: 320
      pdf_page: 344
    - "no": 5
      title: APPLICATION TO LINEAR SYSTEMS
      page: 321
      pdf_page: 345
    - "no": 6
      title: SMALLEST FIELD OF RATIONALITY
      page: 322
      pdf_page: 346
    - "no": 7
      title: CRITERIA FOR RATIONALITY
      page: 323
      pdf_page: 347
statements: 17
exercises: 5
content_sha256: 9d5c3e84851dc723d491ab22b3cba114d9fb1f1ba10106d1f690994b37ea3410
translated_from: content/en/alg/II/08_s8_restriction_of_the_field_ofscalars_in.md
translation_method: google
source_content_sha256: 2ed7e12b55c05b782b900415fee46ae7d943593ea0d536d23f816f7a0166f2be
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: f21b3a40c9bb771a994662e5b87ea00289a3997e4404562d05dff999e4412669
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 8。 ベクトル空間のスカラーの体のうち制限

この段落全体を通じて、K は K の体と K' 部分体を表します。 集合 V では、K 定義する上の右 (それぞれ左) ベクトル空間構造がスカラーの制限により、右 (それぞれ左) ベクトル空間になります。 K'を超える構造。

### 1. K'-構造の定義

#### 命題 1 {#alg-ii-s8-prop-1 .statement tag=05V0}

V を K 上の右ベクトル空間とし、V' を K' 上のベクトル部分空間である V の部分集合とします。 次の条件は同等です。

(a) $V'_{(K)} = V' \otimes_{K'} K$ の K-線型写像 $\lambda$ を V に変換し、すべての $x' \in V', \xi \in K$ に対して $\lambda(x' \otimes \xi) = x'\xi$ が全単射となるようにします。

(b) V' のベクトル K 空間 W へのすべての K' 線形写像 $f'$ は、W への V の K-線型写像 f に一意に拡張できます。

(c) K' 上の V' のすべての基底は、K 上の V の基底です。

(d) K' 上に V' の基底が存在し、これは K 上に V の基底も存在します。

(e) ベクトル K 空間 V は V' によって生成され、K' 上で自由な V' のすべての部分集合は K 上で自由になります。

私たちは、$V'_{(K)}$ が正しいベクトル K 空間構造を持ち、その下に $(x' \otimes \xi)\eta = x' \otimes (\xi\eta)$ (K で $\xi, \eta$、$x' \in V'$) があり、すべての K' 線形マッピングについて V の $f'$ がベクトル K 空間にあることを知っています (§ 5, no. 1)。 W では、$x' \in V'$ に対して $\bar{f}'(x' \otimes 1) = f'(x')$ となるような、$V'_{(K)}$ の K-線型写像 $\bar{f}'$ が W に 1 つだけ存在します。 j が V の標準単射を V にすると、$\lambda$ はちょうど対応する K-線型写像 $\bar{j}$ になります。 $\lambda$ が全単射の場合、すべての K' 線形写像について、$f': V' \to W, \bar{f}' \circ \lambda^{-1}$ は $f'$ を拡張する W への V の一意なK-線型写像になります。その他の語では、(a) は (b) を意味します。 逆に、(b) が成り立つ場合、$V'_{(K)}$ には、すべての $x' \in V'$ に対して $\mu(x') = x' \otimes 1$ となるように、V の特に K-線型写像 $\mu$ が存在します。 $\mu \circ \lambda = 1_{V'_{(K)}}$ は明らかです。一方、すべての $x' \in V'$ に対する $\lambda(\mu(x')) = x'$ と、仮定 $j: V' \to V$ は、V の自己準同型に一意に拡張でき、必然的に $\lambda \circ \mu = 1_V$ となり、(a) と (b) が同等であるという証明が完成します。

K' 上の V' の基底 B' ごとに、$V'_{(K)}$ の元 $v' \otimes 1$ の集合 B ($v'$ が B' を通過する) は、K 上の $V'_{(K)}$ の基底 (§ 5, no. 1, 命題 4) と $\lambda(B) = B'$。 $\lambda$ が全単射であるためには、$V'_{(K)}$ のすべての基底の $\lambda$ の下の像が K 上の V の基底であることが必要であり、$V'_{(K)}$ の 1 つの基底が全単射であれば十分です。 (§ 1, no. 11、系 2 ～ 命題 17)。これにより、(a)、(c)、(d) の同値が証明されます。

K' 上で自由な V' のすべての部分集合は、K' 上で V' の基底に含まれるため (§ 7, no. 1、定理 2)、(c) は (e) を意味します。最後に、(e) が成り立つと仮定します。 B' が K' 上の V' の基底である場合、それは K 上の V のフリーの部分集合です。一方、B' 生成する V' は K' を上回り、したがって生成する V は K を仮定上回ります。したがって、B' は K 上の V の基底であり、これは (e) が (c) を意味していることを証明します。

#### 定義 1 {#alg-ii-s8-def-1 .statement tag=05V1}

*V を体 K および K の K' 部分体上の右ベクトル空間とします。 V 満たすのすべてのベクトルサブ K' 空間 V' は、命題 1 に相当する条件を K' 構造と呼びます。 V.*

#### 例 {#alg-ii-s8-n1-exa-1 .statement tag=05V2}

B を K 上の V の基底とします。K の *すべての* 部分体 K' について、B によって生成された V のベクトルサブ K' 空間は、B を K' 上の基底として認め、したがって V 上の K' 構造になります。 *たとえば、K が可換で、V が多項式 K-代数 K[X_1, ..., X_n] であるとすると、K の部分体 K' ごとに、K'[X_1, ..., X_n] は V 上の K' 構造になります。*

### 2. 部分空間の合理性

#### 定義 2 {#alg-ii-s8-def-2 .statement tag=05V3}

*V を K 上の右ベクトル空間とし、K'-構造 V' とします。 V のベクトルは、属するから V' であれば、K' よりも有理であると言われます。 V のベクトル部分 K 空間 W は、K' に対して有理数であるベクトルによって (K に対して) 生成される場合、K' に対して有理であると言われます。

(v'_i)_{i \in I} を K' 上の V' の基底とします。したがって、これは K 上の V の基底です (no. 1, 命題 1)。 V のベクトル x = $\sum_i v'_i \xi_i$ が K' に関して有理であるためには、すべての $i \in I$ に対して $\xi_i \in K'$ であることが必要かつ十分です。

W が K' 上で *有理* である V のベクトルサブ K 空間である場合、定義 2 から、$W' = W \cap V'$ は W のベクトルサブ K' 空間であり、K 上の *生成する* W であることがわかります。一方、K' 上で自由な W' のすべての部分集合は、V' (no. 1, 命題 1) に含まれるため、K 上でも自由になります。 (no. 1, 命題 1) ということは、W' は、V 上の K'-構造 V' によって *誘導* されたと言われている W 上の *K'-構造* であるということになります。

V' のすべてのベクトル サブ K' 空間 W' について、W' の要素と K の係数の線形結合で構成される V のベクトル サブ K 空間を W'.K で表すものとします。

#### 命題 2 {#alg-ii-s8-prop-2 .statement tag=05V4}

*V を K 上の右ベクトル空間とし、V' を V 上の K' 構造とします。 写像 W' \mapsto W'.K は、V' のベクトルサブ K' 空間の集合のうち全単射であり、K' に対して有理である V のベクトルサブ K' 空間の集合上にあり、逆全単射は W です\mapsto W \cap V'._

明らかに全単射 $\lambda^{-1}: V \to V' \otimes_{\mathbf{K'}} \mathbf{K}$ は、no. 1、命題 1、写像でV' の像のベクトルサブ K' 空間 W' ごとに定義された全単射 $\lambda$ の逆です。 標準単射 $x' \mapsto x' \otimes 1$ と W'.K から W' $\otimes_{\mathbf{K'}} \mathbf{K}$;したがって、命題 2 の主張は、定義 2 の帰結と § 7, no. 9、命題 19 になります。

#### 系 1 {#alg-ii-s8-prop-2-cor-1 .statement tag=05V5}

*K' に対して有理数である V のベクトルサブ K 空間のすべての和とすべての共通部分は、K' に対して有理数部分空間です*。

和に関する主張は明らかです。一方、$(W'_i)_{i \in I}$ が$V'$ の$\mathbf{K}'$ 部分空間のベクトル族である場合、$\left( \bigcap_{i \in I} W'_i \right) \otimes_{\mathbf{K}'} \mathbf{K} = \bigcap_{i \in I} (W_i \otimes_{\mathbf{K}'} \mathbf{K})$ (§ 7, no. 7、系 ～ 命題 14) となり、系が証明されます。

$\mathbf{K}$ に対する $V$ の基底 $B$ は、$\mathbf{K}'$ に対して有理であるベクトルで構成されている場合、$\mathbf{K}'$* に対して *有理であると言われます。

#### 系 2 {#alg-ii-s8-prop-2-cor-2 .statement tag=05V6}

*$\mathbf{K}'$ に対して有理である $V$ の $\mathbf{K}$ のすべての基底は、$\mathbf{K}'$ に対する $V'$ の基底です。

$W'$ が $B$ によって生成された $V'$ のベクトル部分$\mathbf{K}'$ 空間である場合、命題 2 により $W'.\mathbf{K} = V = V'.\mathbf{K}$ となり、そこから$V' = W'$ になります。

### 3. 線形写像の合理性

#### 定義 3 {#alg-ii-s8-def-3 .statement tag=05V7}

*$V_1, V_2$ を $\mathbf{K}$ 上の 2 つの右ベクトル空間とし、それぞれ $\mathbf{K}'$ 構造 $V'_1, V'_2$ を持たせます。 $\mathbf{K}$ 線形写像 $f : V_1 \to V_2$ は、$f(V'_1) \subset V'_2$ の場合、$\mathbf{K}'$ よりも有理であると言われます。*

$V_3$ が $\mathbf{K}$ の 3 番目の右ベクトル空間で、$\mathbf{K}'$ 構造 $V'_3$ と $\mathbf{K}$ 線形写像 $g : V_2 \to V_3$ が $\mathbf{K}'$ に対して有理である場合、明らかに $g \circ f : V_1 \to V_3$ は $\mathbf{K}'$ に対して有理です。

#### 命題 3 {#alg-ii-s8-prop-3 .statement tag=05V8}

*$V_1, V_2$ を、$\mathbf{K}$ 上の 2 つの右ベクトル空間と、$V_1, V_2$ 上の $V'_1, V'_2$ $\mathbf{K}'$ 構造とします。 $V_1$ (それぞれ $V_2$) は、標準的に $V'_1 \otimes_{\mathbf{K}'} \mathbf{K}$ (それぞれ $V'_2 \otimes_{\mathbf{K}'} \mathbf{K}$) (no. 1、命題 1) と識別されます。

(i) *写像 $f' \mapsto f' \otimes 1_{\mathbf{K}} = f'_{(\mathbf{K})}$ は、$\mathrm{Hom}_{\mathbf{K}'}(V'_1, V'_2)$ の全単射から $\mathbf{K}$ の集合への $V_1$ から $V_2$ への線形写像であり、$\mathbf{K}'$ よりも有理です。 逆全単射は、$f$ から $V'_1$ までの制限と同じグラフを持つ、$\mathbf{K}'$ に対するすべての $\mathbf{K}$ 線形マッピング $f : V_1 \to V_2$ と、$\mathbf{K}'$ 線形マッピング $f' : V'_1 \to V'_2$ に関連付けられます。

(ii) *$\mathbf{K}'$ に対するすべての $\mathbf{K}$ 線形写像 $f : V_1 \to V_2$ 有理数について、

$$
f(V'_1) = f(V_1) \cap V'_2 \quad \text{and} \quad f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f).
$$

(i) 上記の識別から明らかに、$f' : V'_1 \to V'_2$ が$\mathbf{K}'$ 線形写像である場合、$f'_{(\mathbf{K})} = f' \otimes 1_{\mathbf{K}}$ は$\mathbf{K}'$ に対して有理であり、$f'$ は$f'_{(\mathbf{K})}$ から$V'_1$ の制限と同じグラフを持つ写像です。逆に、$f : V_1 \to V_2$ が $\mathbf{K}'$ に対する $\mathbf{K}$ 線形写像有理であり、$f' : V'_1 \to V'_2$ が $f$ から $V'_1$、$f$ および $f'_{(\mathbf{K})}$ 一致するの制限と同じグラフを持つ場合、 $V'_1$、つまり$V_1$の$\mathbf{K}$を超えた生成する系なので、$f = f'_{(\mathbf{K})}$になります。

(ii) $f = f' \otimes 1_{\mathbf{K}}$ の場合は、$f(V_1) = f(V'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(V'_1) \otimes_{\mathbf{K}'} \mathbf{K}$ となり、$f'(V'_1) \subset V'_2, f(V'_1) = f'(V'_1) \cap V'_2$ (§ 7, no. 9、命題 19) となります。 公式 $f^{-1}(V'_2) = V'_1 + \mathrm{Ker}(f)$ がすぐに続きます。

#### 系 1 {#alg-ii-s8-prop-3-cor-1 .statement tag=05V9}

命題 3、$\operatorname{Im}(f) = (\operatorname{Im}(f'))_{(\mathbf{K})}$ の記法、
$$
\operatorname{Ker}(f') = (\operatorname{Ker}(f'))_{(\mathbf{K})}, \quad \operatorname{Coker}(f) = (\operatorname{Coker}(f'))_{(\mathbf{K})}.
$$
特に、$f$ が単射法 (それぞれ全単射法、零) であるためには、$f'$ がそうであることが必要かつ十分です。 $f$ が全単射である場合、その逆数写像は $\mathbf{K}'$ に対して有理数です。

これは、§ 7, no. 9、系 ～ 命題 18 の特別なケースです。

#### 系 2 {#alg-ii-s8-prop-3-cor-2 .statement tag=05VA}

$f : V_1 \to V_2$ を $\mathbf{K}'$ に対する有理数の $\mathbf{K}$ 線形写像とする。 For every vector sub-$\mathbf{K}$-space $W_1$ of $V_1$ (resp. $W_2$ of $V_2$) rational over $\mathbf{K}'$, $f(W_1)$ (resp. $f^{-1}(W_2)$) is a vector sub-$\mathbf{K}$-space of $V_2$ (resp. $V_1$) rational over $\mathbf{K}'$.

命題 3 の記法では、$V'_1$、$f'_{(\mathbf{K})}(W'_1 \otimes_{\mathbf{K}'} \mathbf{K}) = f'(W'_1) \otimes_{\mathbf{K}'} \mathbf{K}$ のベクトルサブ$\mathbf{K}'$ スペース $W'_1$ ごとに。 $W_1$ (no. 2、命題 2) に関連するよって主張。 一方、$W'_2$ を $V'_2$ のベクトルサブ$\mathbf{K}'$ 空間とし、$g'$ を正規の $\mathbf{K}'$ 線形写像 $V'_2 \to V'_2/W'_2$ とします。次に$f'(W'_2) = \operatorname{Ker}(g' \circ f')$;したがって、系 1 より、
$$
{f'_{(\mathbf{K})}}^{-1}(W'_2 \otimes_{\mathbf{K}'} \mathbf{K}) = {f'}^{-1}(W'_2) \otimes_{\mathbf{K}'} \mathbf{K},
$$
そこから$W_2$に関する主張が始まります。

$V_1, V_2$ を、それぞれ $\mathbf{K}'$ 構造 $V'_1, V'_2$ を持つ 2 つの正しいベクトル $\mathbf{K}$ スペースとします。 $V'_1 \times V'_2$が$V_1 \times V_2$上の$\mathbf{K}'$構造であるのは明らかであり、$\mathbf{K}'$構造$V'_1$と$V'_2$の積と呼ばれます。

#### 命題 4 {#alg-ii-s8-prop-4 .statement tag=05VB}

$\mathbf{K}$ 線形写像 $f : V_1 \to V_2$ が $\mathbf{K}'$ に対して有理的であるためには、そのグラフ $\Gamma$ が $V_1 \times V_2$ 上の積 $\mathbf{K}'$ 構造に対して $\mathbf{K}'$ に対して有理的であることが必要かつ十分です。

$g$ を $V_1$ から $V_1 \times V_2$ までの写像 $x_1 \mapsto (x_1, f(x_1))$ とします。これは、$\Gamma = g(V_1)$ のような $\mathbf{K}$ 線形マッピングです。 $f$ が $\mathbf{K}'$ に対して有理である場合、系 2 から命題 3 のおかげで、$\Gamma$ も同様です。 逆に、$\Gamma$ が $\mathbf{K}'$ に対して有理であると仮定し、$V_1 \times V_2$ の構造によって誘発される $\mathbf{K}'$ 構造を持つとします。 定義からすぐに、射影 $\mathrm{pr}_1, \mathrm{pr}_2$ の制限 $p_1, p_2$ から $\Gamma$ は、$\Gamma$ の $\mathbf{K}'$ から $V_1$ に対して有理である $\mathbf{K}$ 線形写像であることがわかります。それぞれ$V_2$。 $p_1$ は全単射なので、その逆数写像 $q_1$ は $\mathbf{K}'$ (系 1 から命題 3) に対して有理であり、したがって $f = p_2 \circ q_1$ も同様です。

### 4. 合理的線型形式

$V$ を $\mathbf{K}'$ 構造 $V'$ で $\mathbf{K}$ の上に右ベクトル空間とする。 $K'_d$ は右側のベクトル $\mathbf{K}$-空間 $K_d$ の $\mathbf{K}'$ 構造であるため、$V$ の線形写像として、$\mathbf{K}'$ に対して有理数で定義する線型形式 $x^* \in V^*$ を得ることができます。 $K_d$、$\mathbf{K}'$ よりも合理的

V と K_d の K'-構造。 no. 3、命題 3、集合により、これら線型形式の R' は、合成写像の下で V' の双対 V'* の像になります。

(I) $$ {V'}^* \xrightarrow{\phi} K \otimes_{K'} {V'}^* \xrightarrow{\upsilon} V^* $$

ここで、$\phi({x'}^*) = 1 \otimes {x'}^*$ と $\upsilon(\xi \otimes {x'}^*)$ は、V では線型形式 $y^*$ となり、すべての $x' \in V'$ (§ 5, no. 4) に対して $y^*(x') = \xi \langle {x'}^*, x' \rangle$ になります。この写像は単射 (§ 7, no. 9、命題 20 および 19) であり、明らかに R' は V* の左ベクトルサブ K' 空間であることがわかっています。さらに、K' 上で自由な R' のすべての部分集合は K 上で自由です。しかし、一般に R' は必ずしも K 上で生成する V* であるとは限らず、したがって V* (練習問題 2) 上で定義する K' 構造を形成することはありません。ただし、V が K 上の有限次元 n であり、V'* が K' および R' 上の次元 n である場合、定義するは正準的に V* 上の K'-構造になります。

#### 命題 5 {#alg-ii-s8-prop-5 .statement tag=05VC}

V を K 上の右ベクトル空間、V' を V 上の K' 構造、および V の W ベクトルサブ K 空間とします。 W が K' 上で有理数であるためには、W が V (§ 2, no. 4) における H の直交となるように、K' 上で有理数線型形式の集合 H \部分集合 V^* が存在することが必要かつ十分です。

H を元が K' に対して有理線型形式である V* の部分集合とします。すべての $x^* \in H$、$x^*$ の核は、V のベクトルサブ K 空間であり、K' 上の有理数です (no. 3、系 2 ～ 命題 3)。したがって、これらの核のうち共通部分は、K' に対して有理数である V の部分 K 空間ベクトルでもあります (no. 2、系 1 ～ 命題 2)。

逆に、W を K' に対して有理数の V のサブ K 空間ベクトルとし、W を $W' \otimes_{K'} K$ と同一視します。ここで、$W' = W \cap V'$ (no. 2, 命題 2) となります。 線型形式 ${x'}^* \in {V'}^*$ が W' 上で零であるためには、no. 3、系 I により、(1) の下で対応するが W 上で零となる線型形式 $x^* \in V^*$ が必要かつ十分です。 命題 3、

$$
\operatorname{Ker}(x^*) = (\operatorname{Ker}({x'}^*)) \otimes_{K'} K \quad \text{and} \quad \operatorname{Ker}(x^{*\prime}) = (\operatorname{Ker}(x^*)) \cap V'.
$$

H' を V'* の W' の直交関数とします。私たちは (§ 7, no. 5, 定理 7) W' が V' における H' の直交であることを知っています。 写像 (1) の下で、H が V* の H' の像である場合、上記から、no. 7、系 ～ 命題 14 を考慮すると、W は V の H の直交であることがわかります。

### 5. リニアへの応用系

#### 命題 6 {#alg-ii-s8-prop-6 .statement tag=05VD}

(i) 均一一次方程式の系が与えられた場合

(2)
$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = 0 \quad (\mu \in M)
$$
その係数 $\alpha_{\mu i}$ が K' に属する場合、K の要素からなるこの系のすべての解 $(\xi_i)$ は、K' の要素からなる (2) の解 $(\xi'_i)$ K の係数との線形結合です。

(ii) *線形方程式の系が与えられた*

$$
\sum_{i \in I} \alpha_{\mu i} \xi_i = \beta_\mu \quad (\mu \in M)
$$

*誰の係数* $\alpha_{\mu i}$ *そして右側* $\beta_\mu$ *属するから* $K'$、 *元の $K$ の解から系からなるが存在する場合、 *解も存在しますからなる/元/* $K'$。

(i) すべての集合 S について、右側のベクトル K 空間 $K_d^{(S)}$ に $K'$ 構造 $K_{d'}^{(S)}$ が与えられるとします。 $f$ を、すべての $\mu \in M$ について $\zeta_\mu = \sum_{i \in I} \alpha_{\mu i} \xi_i$ によって定義されるベクトル $(\xi_i)_{i \in I}$ からベクトル $(\zeta_\mu)_{\mu \in M}$ ごとに、$K_d^{(I)}$ の K-線型写像を $K_d^{(M)}$ 写像にします。明らかに、$f$ は $K'$ よりも合理的です。 系 (2) の K の解の集合である核 V は、$K'$ に対して $K_d^{(I)}$ の部分空間 (no. 3, 系 2 から命題 3) なので、$K'$ の (2) の解によって生成されます。

(ii) K を左のベクトル $K'$-スペースとみなします。 K のベクトル部分空間 $K'_s$ (§ 7, no. 3, 命題 4) 上に K の $K'$ 線形射影子 $p$ が存在します。 $(\xi_i)$ が K の (3) の解である場合、$\sum_{i \in I} \alpha_{\mu i} p(\xi_i) = p \left( \sum_{i \in I} \alpha_{\mu i} \xi_i \right) = p(\beta_\mu) = \beta_\mu$ となり、$(p(\xi_i))$ が $K'$ の (3) の解であることが証明されます。

命題 6 が K と $K'$ に当てはまる場合、環 K は、部分環 $K'$ に対して (左) *忠実にフラット* と呼ばれます。この概念については後で詳しく学習します (*可換代数*、I, § 3)。

### 6. 合理性の最小の体

V を $K'$ 構造 $V'$ を持つ右ベクトル K 空間とします。 $K' \subset L \subset K$ となるすべての体 L に対して、$V_L = V'.L$ と書きます。明らかに、$K'$ を超える $V'$ のすべての基底は、K を超える V の基底と、L を超える $V_L$ の基底です。したがって、$V_L$はVのL構造であり、$V'$は$V_L$の$K'$構造です。

#### 命題 7 {#alg-ii-s8-prop-7 .statement tag=05VE}

(i) *V を K' 構造 V' を持つ右ベクトル K 空間とする。 すべてのベクトル $x \in V$ (それぞれ V のすべてのベクトルサブ K 空間 W)、部分体の集合、K 含む $K'$ の L など、$x$ (それぞれ W) が有理となるものについてL には少なくとも元 $K'(x)$ (それぞれ $K'(W)$) があります。

(ii) *$V_1, V_2$ を、それぞれ K' 構造 $V_1', V_2'$ を持つ 2 つの正しいベクトル K 空間とします。 $V_1$ のすべての K-線型写像 f を $V_2$、部分体の集合、K 含む $K'$ の L に対して、f が L に対して有理数となるように、少なくとも元 $K'(f)$* が得られます。

まず、ベクトル $x \in V$ に対して主張 (i) を証明します。 B を $K'$ に対する V の有理数である基底とします。 B は、体 L ごとに、$K'$ にわたる $V'$ の基底と L にわたる $V_L$ の基底であり、$K' \subset L \subset K$ になります。 $x = \sum_{b \in B} b \xi_b$がLに対して有理であるためには、$\xi_b$属するからL(no. 2)、したがって最小の体Lとこの性質が成り立つことが必要かつ十分です。 体 *生成* は K' によって、$\xi_b$ は $b \in B$ 用です。

次に(ii)を証明します。 $B_1, B_2$ を、それぞれ $K'$ に対して有理である $V_1, V_2$ の基底とし、すべての $b_1 \in B_1, f(b_1) = \sum_{b_2 \in B_2} b_2 \alpha_{b_2 b_1}$ について書きます (*ファミリー $(\alpha_{b_2 b_1})$ は、基底 $B_1$ と $B_2$; cf. に関する $f$ の * 行列* にすぎません) § 10, no. 4*)。 $B_1$ (それぞれ $B_2$) は、$K' \subset L \subset K$ などの各フィールドの L に対する $(V_1)_L$ (それぞれ $(V_2)_L$) の基礎であるため、$f$ が L に対して有理であるためには、$\alpha_{b_2 b_1}$ が以下に属することが必要かつ十分です。 L;したがって、このプロパティを持つ最小のフィールドは、K' と $b_1 \in B_1, b_2 \in B_2$ の $\alpha_{b_2 b_1}$ によって *生成* されたフィールドです。

最後に、V の部分空間 W に対して主張 (i) を確立するには、まず次の補題を証明します。

#### 補題 1 {#alg-ii-s8-lem-1 .statement tag=05VF}

*V を K' 構造 V' と W ベクトルサブ K 空間 V を持つ右ベクトル K 空間とします。 V の 2 つのベクトルサブ K 空間 $W_1, W_2$ が存在し、K' に対して有理で、V が $W_1$ と $W_2$ の直和となり、V が $W_1 \times W_2$ と同一視される場合、W は次のグラフになります。 $W_1$ を $W_2$ にK-線型写像 g。*

B を K' に対して有理数の V の基底とします。 § 7, no. 1 の適用定理 2、W over K の基底は、V のフリー 部分集合と、このフリー 部分集合の生成する系和集合と B が存在することがわかります。 V が W の直和および C によって生成された V の部分空間 $W_2$ となるような B の部分集合 C。 また、$W_1$ を、$B - C$ によって生成された V の部分空間とします。 $B \subset V'$ のように、明らかに $W_1$ と $W_2$ は K' に対して有理です。 さらに、すべての $x \in W_1$ に対して、V は W と $W_2$ の直接和であるため、$x + g(x) \in W$ となる $W_2$ のベクトル $g(x)$ が 1 つだけ存在します。この場合、W は g のグラフであり、W は V のベクトル部分 K 空間であるため、g は K 線形です。

これを補題証明したので、g が L (no. 3, 命題 4) に対して有理である場合に限り、K 含む K' の部分体 L に対して W が有理であることが知られています。 g が $K'(g)$ に対して有理であるような最小の体 $K'(g)$ は、したがって、W が有理である最小の体でもあります。

### 7. 合理性の基準

K のすべての部分体 L について、$\mathrm{End}_L(K)$ は、L 上の *左ベクトル空間* とみなされる K の自己準同型環を表します。 L 含む K' の場合、$\mathrm{End}_L(K)$ は $\mathrm{End}_{K'}(K)$ の部分環です。 $\mathrm{End}_{K'}(K)$ のすべてのサブセット $\mathscr{M}$ について、K' を含む K の *最大サブフィールド * L が存在し、そのような $\mathscr{M}$ は $\mathrm{End}_L(K)$ に含まれます。つまり、すべての $\eta \in K$ とすべての $\phi \in \mathscr{M}$ に対して $\phi(\xi \eta) = \xi \cdot \phi(\eta)$ となるような $\xi \in K$ のセットです (次のことがすぐに検証されます)。この集合は環であり、一方、前述の関係式の $\eta$ を $\xi^{-1} \eta$ に置き換えると、$\xi \neq 0$ のとき $\phi(\xi^{-1} \eta) = \xi^{-1} \cdot \phi(\eta)$ が得られます。 このフィールドを K の $\mathscr{M}$ の *centralizer* と呼び、$\chi(\mathscr{M})$ で表すことにします。

ここで、V を K' 構造 V' を持つ右ベクトル K 空間とします。 For all $\phi \in \mathrm{End}_{K'}(K)$, there exists one and only one endomorphism $\phi_v$ of the $\mathbf{Z}$-module V such that $\phi_V(x'.\xi) = x'.\phi(\xi)$ for $x' \in V'$ and $\xi \in K$: for, in no. 1, a $\mathbf{Z}$-isomorphism $\lambda$ of $V' \otimes_{K'} K$ onto V was defined which maps $x' \otimes \xi$ to $x'.\xi$ and $\phi_V$ is necessarily equal to $\lambda \circ (1_{V'} \otimes \phi) \circ \lambda^{-1}$.

#### 定理 1 {#alg-ii-s8-thm-1 .statement tag=05VG}

*$\mathscr{M}$ を $\mathrm{End}_{K'}(K)$ の部分集合および $\mathscr{M}$ の集中化者である K の $L = \chi(\mathscr{M})$ 部分体とします。

(i) *V を K' 構造を持つ右側のベクトル K 空間とする。 ベクトル $x \in V$ が L に対して有理であるためには、すべての $\phi \in \mathscr{M}$ とすべての $\eta \in K$ に対して $\phi_V(x.\eta) = x.\phi(\eta)$ であることが必要かつ十分です。 V のベクトルサブ K 空間 W が L に対して有理であるためには、すべての $\phi \in \mathscr{M}$ に対して $\phi_V(W) \subset W$ であることが必要かつ十分です。*

(ii) *$V_1, V_2$ を、それぞれ K' 構造を持つ 2 つの正しいベクトル K 空間とします。 $V_1$ から $V_2$ への K-線型写像が L に対して有理であるためには、すべての $x_1 \in V_1$ とすべての $\phi \in \mathscr{M}$ に対して $f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))$ であることが必要かつ十分です。

まず、x について主張 (i) を証明します。 B を K' に対する V の有理数の基底とし、$x = \sum_{b \in B} b.\xi_b$ と書きます。次に、$\phi \in \mathscr{M}$ と $\eta \in K$ については、

$$
\phi_V(x.\eta) - x.\phi(\eta) = \sum_{b \in B} b.(\phi(\xi_b\eta) - \xi_b.\phi(\eta))
$$

したがって、関係

「すべての$\phi \in \mathscr{M}$とすべての$\eta \in K$、$\phi_V(x.\eta) = x.\phi(\eta)$のために」

そして

「すべての$\phi \in \mathscr{M}$、すべての$b \in B$、およびすべての$\eta \in K$、$\phi(\xi_b\eta) = \xi_b.\phi(\eta)$」

は同等です。これらの 2 番目の関係は、すべての $b \in B$、$\xi_b \in \chi(\mathscr{M})$ について、(i) の最初の主張を証明します。

次に(ii)を証明します。 f が L 上で有理数であるためには、K' 上ですべての $x'_1 \in V_1$ 有理数に対して、$f(x'_1)$ が L 上で $V_2$ 有理数内のベクトルであることが必要かつ十分です。これは、L に対して有理数である $V_1$ のすべてのベクトル $x_1$ について、$f(x_1)$ が L に対して有理であることを意味します。そのようなベクトルは、K' に対して有理数であるベクトルの L の係数との線形結合です。 上記の条件は、引数の最初の部分により、 関係と同等です。

$$
f(x'_1).\phi(\eta) = \phi_{V_2}(f(x'_1).\eta) \quad \text{for } \phi \in \mathscr{M} \text{ and } \eta \in K
$$

これも書かれているかもしれません

$$
f(\phi_{V_1}(x'_1.\eta)) = \phi_{V_2}(f(x'_1.\eta)) \quad \text{for } \phi \in \mathscr{M} \text{ and } \eta \in K.
$$

$V_1$ のすべての元は、K' に対して有理数の $V_1$ の元の K に係数が含まれる線形結合であるため、条件 (5) は次と同等です。

$$
f(\phi_{V_1}(x_1)) = \phi_{V_2}(f(x_1))
$$

すべての $x_1 \in V_1$ とすべての $\phi \in \mathscr{M}$ に対して。

最後に、(i) の 2 番目の主張を証明するために、no. 6, 補題 1 を使用します。W は K-線型写像 $g : W_1 \to W_2$ のグラフであり、写像 g が L (no. 3, 命題 4) に対して有理である場合に限り、W は有理です。 (ii) により、g が L に対して有理であるためには、すべての $x_1 \in W_1$ とすべての $\phi \in \mathscr{M}$ に対して $g(\phi_{W_1}(x_1)) = \phi_{W_2}(g(x_1))$ であることが必要かつ十分です。 $\phi_v = \phi_{W_1} \times \phi_{W_2}$ のように、上記の条件は、g のグラフ W がすべての $\phi \in \mathscr{M}$ について $\phi_v$ 以下で安定していることを意味します。

### 練習問題 {#alg-ii-s8-exercises}

[§ 8 に対して練習問題](exercises/s8/)を参照してください。
