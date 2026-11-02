---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 4
section_title: Flat modules and "Tor" functors
lang: ja
source: ac-i-vii
book_pages: 37-38, 50
pdf_pages: 0057-0058, 0070-0070
extraction: ocr
statements: 3
exercises: 1
content_sha256: 4add6e3869515dd48fbb5fd8c3bccea71662a59da55fa875e0f6d19255104aaf
translated_from: content/en/ac/I/04_s4_flat_modules_and_tor_functors.md
translation_method: google
source_content_sha256: 2e67efa01c1410cffb73e90e94fea2974820179f25619519676ed3aa28003654
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-eeeca2ef
glossary_version: 34
glossary_terms_sha256: 89b7b6f3ce91ceef22b7331e25c0975f864900f109f2893f2d5b698252a40bea
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 4. フラット加群と「tor」ファンクター

ホモロジー 代数 (*) に精通している読者の利益のために、フラット加群の理論が Tor ファンクターのそれとどのように関連しているかを簡単に示します。

#### 命題 1 {#ac-i-s4-prop-1 .statement tag=044W}

Eを右A-加群とします。次の 4 つのプロパティは同等です。

(a) E はフラットです。
(b) すべての左A-加群 F およびすべての整数 n $\geq 1$、$\mathrm{Tor}_n^A(E, F) = 0$ について。
(c) 左A-加群 F ごとに、$\mathrm{Tor}_1^A(E, F) = 0$。
(d) A の有限生成された左イデアル $a$ ごとに、
$$
\mathrm{Tor}_1^A(E, A_s/a) = 0.
$$

(a) が (b) を意味することを示します。しましょう
$$
\cdots \to L_n \to L_{n-1} \to \cdots \to L_0 \to F \to 0
$$
F の自由解像度になります。E はフラットなので、数列
$$
(1) \quad \cdots \to E \otimes L_n \to E \otimes L_{n-1} \to \cdots \to E \otimes L_0 \to E \otimes F \to 0
$$
正確です。 $\mathrm{Tor}_n^A(E, F)$ は複合体 (1) の相同性群と同型であるため、$n \geq 1$ に対して零です。 (b) が (c) を意味し、(c) が (d) を意味することは自明です。最後に、(d) が (a) を意味することを示します。 完全系列
$$
0 \to a \to A, \to A_s/a \to 0
$$
完全系列を与えます
$$
\mathrm{Tor}_1^A(E, A_s/a) \to E \otimes_A a \to E \otimes_A A.
$$
(d) が成り立つので、標準準同型
$$
E \otimes_A a \to E \otimes_A A = E
$$
は単射です。これは、E がフラット (§ 2, no. 3, 命題 1) であることを意味します。

命題 1 は、アプリケーションで役立つことが多いフラット加群の特徴付けを提供します。私たちは、例によって、

(*) カテゴリー、特に (準備中) のアーベルカテゴリーに特化したこの論文の部分を参照してください。これが出版されるまで、読者は H. CARTAN-S に問い合わせることができます。 EILENBERG、Homological 代数、プリンストン、1956 年、または R. GODEMENT、Théorie des Faisceaux、パリ (Hermann)、1958 年。

$$
\operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E'', F)
$$

は、左A-加群 F ごとに $\operatorname{Tor}_1^A(E, F) = 0$ を示しているため、E はフラットです。 E と E'' が平坦な場合、完全系列

$$
\operatorname{Tor}_2^A(E'', F) \to \operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F)
$$

は $\operatorname{Tor}_1^A(E', F) = 0$ を示しているため、E' はフラットです。

#### 命題 2 {#ac-i-s4-prop-2 .statement tag=044X}

*R、S を 2 つの環、$\rho : \mathbf{R} \to \mathbf{S}$ 準同型、F を左の R モジュールとします。次の 2 つのプロパティは同等です:*
(a) 右側の S モジュール E ごとに $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$。
(b) *左の S モジュール $\varphi^*(F) = F_{(S)} = S \otimes_R F$ は平坦で、$\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$ です。*

(a) が成り立つとします。 $E = S_d$ を取ると、$\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$ であることがわかります。 $F_{(S)}$ がフラット S 加群であることも示します。そのため、E が正しい S モジュールである場合、加法群 $E \otimes_S F_{,,}$ は $\rho_*(E) \otimes_R F$ と識別されることに注意してください。次に、正しい S モジュールが完全系列ある場合

$$
0 \to E' \to E \to E'' \to 0
$$

(a) を使用して、完全系列を取得します。

$$
0 \to \rho_*(E') \otimes_R F \to \rho_*(E) \otimes_R F \to \rho_*(E'') \otimes_R F \to 0
$$

またはまた

$$
0 \to E' \otimes_S F_{(S)} \to E \otimes_S F_{(S)} \to E'' \otimes_S F_{(S)} \to 0
$$

これは、$F_{(S)}$ が平坦であることを証明します。

逆に、(b) が成り立つ場合、まず、すべての *空き* 正しい S モジュール $L = S_d^{(I)}$、$\operatorname{Tor}_1^R(\rho_*(L), F) = (\operatorname{Tor}_1^R(\rho_*(S_d), F))^{(I)} = 0$ が得られます。適切なすべての S モジュール E は、適切な空き S モジュール L のために形 $E = L/H$ に書き込むことができます。それなら完全系列です

(2) $0 = \operatorname{Tor}_1^R(\rho_*(L), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.$

しかし、$F_{,,}$ は平坦であるため、準同型 $H \otimes_S F_{(S)} \to L \otimes_S F_{(S)}$ は単射法であり、準同型と同一視されます。

$$
\rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.
$$

すると(2)から$\operatorname{Tor}_1^R(\rho_*(E), F) = 0$となります。

#### 注意 {#ac-i-s4-n0-rem-1 .statement tag=044Y}

命題 2 も完全系列の存在から導かれます

$$
E \otimes_S \operatorname{Tor}_1^R(\rho_*(S_d), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \operatorname{Tor}_1^S(E, S_d \otimes_R F) \to 0
$$

Tor 関手の「結合性」のスペクトル数列から生じます。

### 練習問題 {#ac-i-s4-exercises}

[§ 4 に対して練習問題](exercises/s4/)を参照してください。
