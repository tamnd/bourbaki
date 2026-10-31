---
book: ac
book_title: Commutative Algebra
chapter: I
chapter_title: FLAT MODULES
section: 4
section_title: Flat modules and "Tor" functors
lang: zh
source: ac-i-vii
book_pages: 37-38, 50
pdf_pages: 0057-0058, 0070-0070
extraction: ocr
statements: 3
exercises: 1
content_sha256: 34cdd7c4a11d2923d23eae71a5a3eee5f96f3d51fafac159792fb359a6e63cda
translated_from: content/en/ac/I/04_s4_flat_modules_and_tor_functors.md
translation_method: google
source_content_sha256: 2e67efa01c1410cffb73e90e94fea2974820179f25619519676ed3aa28003654
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: f8934e29f1c56fbc40cf232cf4d7d987edd6f7ddb3e6098adb4614f1aa7ca586
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## 4. Flat 模和“TOR”函子

为了方便熟悉同调代数 (*) 的读者，我们将快速指出平直模的理论与 Tor 函子理论的关系。

#### 命题 1 {#ac-i-s4-prop-1 .statement tag=044W}

令 E 为右A-模。以下四个属性是等效的：

(a) E 是平的。
(b) 对于每个左A-模 F 和每个整数 n $\geq 1$，$\mathrm{Tor}_n^A(E, F) = 0$。
(c) 对于每左A-模 F，$\mathrm{Tor}_1^A(E, F) = 0$。
(d) 对于 A 的每个有限生成的左理想 $a$，
$$
\mathrm{Tor}_1^A(E, A_s/a) = 0.
$$

我们证明（a）蕴涵（b）。让
$$
\cdots \to L_n \to L_{n-1} \to \cdots \to L_0 \to F \to 0
$$
是 F 的自由分辨率。由于 E 是平坦的，序列
$$
(1) \quad \cdots \to E \otimes L_n \to E \otimes L_{n-1} \to \cdots \to E \otimes L_0 \to E \otimes F \to 0
$$
是准确的。由于$\mathrm{Tor}_n^A(E, F)$与配合物(1)的同源群同构，因此对于$n \geq 1$来说，它们是零。 (b) 暗示(c) 且(c) 暗示(d) 是微不足道的。最后我们证明（d）蕴涵（a）。 正合序列
$$
0 \to a \to A, \to A_s/a \to 0
$$
给出正合序列
$$
\mathrm{Tor}_1^A(E, A_s/a) \to E \otimes_A a \to E \otimes_A A.
$$
由于 (d) 成立，典范同态
$$
E \otimes_A a \to E \otimes_A A = E
$$
是单射的，这意味着 E 是平坦的 (§ 2, no. 3, 命题 1)。

命题 1 提供了模的刻画，这在应用中通常很有用。我们将通过例来限制自己，以给予

(*) 请参阅本论文的部分，专门讨论类别，特别是阿贝尔的类别（正在准备中）。在本文出版之前，读者可以查阅 H. CARTAN-S。 EILENBERG，同源代数，普林斯顿，1956 年，或 R. GODement，Théorie des Faisceaux，巴黎（赫尔曼），1958 年。

$$
\operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F) \to \operatorname{Tor}_1^A(E'', F)
$$

表明每左A-模 F 都有 $\operatorname{Tor}_1^A(E, F) = 0$，因此 E 是平坦的。如果 E 和 E'' 平坦，正合序列

$$
\operatorname{Tor}_2^A(E'', F) \to \operatorname{Tor}_1^A(E', F) \to \operatorname{Tor}_1^A(E, F)
$$

表明 $\operatorname{Tor}_1^A(E', F) = 0$，因此 E' 是平坦的。

#### 命题 2 {#ac-i-s4-prop-2 .statement tag=044X}

*设 R、S 为两个环、$\rho : \mathbf{R} \to \mathbf{S}$ 同态，F 为左 R 模。以下两个属性是等效的：*
(a) 对于每个右 S 模 E 都有 $\operatorname{Tor}_1^R(\rho_*(E), F) = 0$。
(b) *左 S 模 $\varphi^*(F) = F_{(S)} = S \otimes_R F$ 是平的且 $\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$。*

假设(a)成立。取$E = S_d$，我们看到$\operatorname{Tor}_1^R(\rho_*(S_d), F) = 0$。我们还证明 $F_{(S)}$ 是一个平面 S 模。为此，我们注认为，如果E是右S模，则加法群$E \otimes_S F_{,,}$可以用$\rho_*(E) \otimes_R F$来标识。那么如果有正合序列个右S-模

$$
0 \to E' \to E \to E'' \to 0
$$

我们使用 (a) 得到正合序列

$$
0 \to \rho_*(E') \otimes_R F \to \rho_*(E) \otimes_R F \to \rho_*(E'') \otimes_R F \to 0
$$

或者也

$$
0 \to E' \otimes_S F_{(S)} \to E \otimes_S F_{(S)} \to E'' \otimes_S F_{(S)} \to 0
$$

这证明$F_{(S)}$是平坦的。

相反，如果 (b) 成立，则首先对于每个“自由”右 S 模 $L = S_d^{(I)}$，$\operatorname{Tor}_1^R(\rho_*(L), F) = (\operatorname{Tor}_1^R(\rho_*(S_d), F))^{(I)} = 0$。每个正确的 S 模块 E 都可以写成形式 $E = L/H$，以获得合适的自由 S 模块 L；那么我们就有正合序列

(2) $0 = \operatorname{Tor}_1^R(\rho_*(L), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.$

但由于 $F_{,,}$ 是平的，同态 $H \otimes_S F_{(S)} \to L \otimes_S F_{(S)}$ 是单射的，并且与同态一致

$$
\rho_*(H) \otimes_R F \to \rho_*(L) \otimes_R F.
$$

然后从(2)得出$\operatorname{Tor}_1^R(\rho_*(E), F) = 0$。

#### 注 {#ac-i-s4-n0-rem-1 .statement tag=044Y}

命题 2 也因正合序列的存在而推出

$$
E \otimes_S \operatorname{Tor}_1^R(\rho_*(S_d), F) \to \operatorname{Tor}_1^R(\rho_*(E), F) \to \operatorname{Tor}_1^S(E, S_d \otimes_R F) \to 0
$$

由 Tor 函子“结合性”的光谱序列产生。

### 习题 {#ac-i-s4-exercises}

§ 4](exercises/s4/)参见[习题。
