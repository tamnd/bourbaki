---
book: top
book_title: General Topology
chapter: V
chapter_title: One-parameter groups
section: 3
section_title: Topological characterization of the groups R and T
lang: ja
source: top-v-x
pdf_pages: 0023-0025, 0031-0034
extraction: ocr
statements: 5
exercises: 8
content_sha256: 7daa1545d9e89c30e6ac1d1889d6d6f26066f3467ccf65702b781351e54917ff
translated_from: content/en/top/V/03_s3_topological_characterization_of_the.md
translation_method: google
source_content_sha256: b250fd39401223e4fa03cf5ea015761d2798fe7a40dda8dc19bea27b8a96e356
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: e7f978cfb6584e04094fe37e27c9192cde5c80be0770bc9950badf574d79c98f
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 3. 群 $\mathbf{R}$ および $\mathbf{T}$ のトポロジカル特徴付け

#### 定理 1 {#top-v-s3-thm-1 .statement tag=0BVN}

*トポロジカル群* $G$ *そこには、* $\mathbf{R}$ の開区間と同同型の単位元の近傍が存在し、 * $\mathbf{R}$ と局所的に同型です。

この定理の重要性は、群 $G$ の純粋に位相的な性質から、$G$ の *群構造* の性質を推定できることです。

ここで私たちが懸念しているのは、群 $\mathbf{R}$ に特有であり、$n > 1$ (cf. 章 VIII, § 1, no. 4) のときの群 $\mathbf{R}^n$ に類似する現象ではありません。 $\mathbf{R}$ と局所的に同型の群は、*1 パラメーター 群* と呼ばれるときどきです。

定理 1 を証明するには、簡約するを § 2 の命題 2 にします。 仮説によれば、$G$ の単位元 $e$ の開近傍 $U$ の同相同型性 $\varphi$ が $\mathbf{R}$ の開区間上に存在します。 写像 $\varphi$ の逆関数を使用すると、区間 $\varphi(U)$ の線形位数構造を輸送から $U$ に変換できます。 $U$ の位相 ($G$ のそれによって誘発される) は、$U$ のすべてのオープン区間 (章) のうち基底からなるを持ちます。

IV、 、no. 4、 命題 5)。 V.V ⊂ U となるような e の対称近傍 V と、V が開いた区間であるようなものを見つけることができます。なぜなら、 V'.V' ⊂ U ∩ U^{-1}, V'.V'^{-1} ⊂ U となるような開いた区間 V' 含む e が存在し、 V'^{-1}.V' ⊂U; V = V' ∪ V'^{-1} を取ると、V は開いていて対称で、V.V ⊂ U を満たし、接続されているため、区間 (章 IV, § 2, no. 5, 定理 4)

x、y、z 属するから V の場合、関係 x < y は xz < yz および zx < zy を意味することを示します。確かに、写像 f_1(z) = φ(yz) − φ(xz) と f_2(z) = φ(zy) − φ(zx) は V で連続です。 z = e の場合、それらは > 0 であり、V では消滅しません [たとえば、φ(yz) = φ(xz) の場合、yz = xz となるはずであり、従って y = x]。 f_1(V) と f_2(V) は接続されているため (章 I, § 11, no. 2, 命題 4)、従って R では区間 (章 IV, § 2, no. 5, 定理 4)、そしてこれらはそれぞれ区間であるため、 含む数 > 0 であり、含む 0 ではない場合、それらは R^*_+ に含まれます。つまり、すべての z ∈ V に対して f_1(z) > 0 および f_2(z) > 0 があります。

x と y が V の 2 つの元で、x ≥ e および y ≥ e である場合、特に xy ≥ e になります。 E が e 以上である U の元の (線形順序付け) 集合を表し、I が e より大きい V の元の集合を表すものとします。この場合、§ 2 の公理 (GR_I)、(GR_{II})、(GR_{IIIa})、(GR_{IVa}) が満たされます (ω を元 e とし、合成の法則を群 G のものとします)。 (GR_I)、(GR_{II})、(GR_{IVa}) については、これまでの内容から明らかです。 (GR_{IIIa}) に関しては、e < x < y (x ∈ V, y ∈ V) の場合、x^{-1} ∈ V であるため、x^{-1} < e < x^{-1}y および x^{-1}y < y であることに注意するだけで十分です。従って、z = x^{-1}y 属するから I となり、xz = y となります。従って、§ 2の命題2により、Iの真に増加する写像fがRの区間上に存在し、左側の終点が0となり、x、y、xy属するのときはいつでもf(e) = 0およびf(xy) = f(x) + f(y)になります。から I (これは、x と y 属するから W ∩ I まで、W は e の近傍であり、W.W ⊂ V となる場合に当てはまります)。

I に属さないすべての要素 x ∈ V については、x < e であるため、x^{-1} > e になります。従って、V のすべての x < e に対して $\overline{f}(x) = -f(x^{-1})$ を代入することで、R の区間上で V の厳密に増加する写像 $\overline{f}$ に f を拡張できます。 $\overline{f}(V)$ に含まれるオープン区間の $\overline{f}$ の下の逆像は、V のオープン区間であるため、$\overline{f}$ は V で連続します。逆に、V のオープン区間の $\overline{f}$ の下の像は、$\overline{f}(V)$ のオープン区間であるため、$\overline{f}$ は、群 R の 0 の近傍に対する V の準同型写像です。 一方、x、y、xy がすべて V に属する場合、$\overline{f}(xy) = \overline{f}(x) + \overline{f}(y)$ であることは (§ 1, no. 4 の命題 6 のように、さまざまな考えられる場合を考慮することで) 簡単に確認できます。従って、G の e の適切な近傍に限定された $\overline{f}$ は、G と R の局所同型写像であると結論付けます (III, § 1, no. 3 章、命題 3)。

Q.E.D.

#### 定理 2 {#top-v-s3-thm-2 .statement tag=0BVO}

*接続された群* $G$ *中には、* $\mathbf{R}$ の開区間と同型の単位元の近傍が存在します。 * $\mathbf{R}$ * または* $\mathbf{T}$ のいずれかと同型です。

これは、前の定理の明らか帰結と、§ 1, no. 4 の命題 7 です。

#### 注意 1 {#top-v-s3-rem-1 .statement tag=0BVP}

定理 2 の条件を満たす群 $G$ が $\mathbf{T}$ または $\mathbf{R}$ と同型であるかどうかを判断するには、$G$ がコンパクトかどうかを確認するだけで十分です。

#### 注意 2 {#top-v-s3-rem-2 .statement tag=0BVQ}

定理 2 は、特に、群 $\mathbf{R}$ と *同型* であるすべての位相的群が $\mathbf{R}$ と *必ず同型* であることを示しています。

#### 注意 3 {#top-v-s3-rem-3 .statement tag=0BVR}

群 $\mathbf{R}$ と $\mathbf{T}$ の先行するトポロジカル特徴付けには、補助的な集合としてトポロジカル空間 $\mathbf{R}$ が含まれています。 $\mathbf{R}$ と $\mathbf{T}$ のトポロジカル群構造は、補助的な集合を含まない公理によって特徴付けることが可能です (練習問題 4 と 5 を参照)。

### 練習問題 {#top-v-s3-exercises}

[§ 3 に対して練習問題](exercises/s3/)を参照してください。
