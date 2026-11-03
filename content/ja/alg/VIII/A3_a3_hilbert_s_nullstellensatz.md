---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 3
section_title: Hilbert’s Nullstellensatz
appendix: true
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.461-A VIII.462
pdf_pages: 0478-0479
extraction: native
statements: 3
exercises: 0
content_sha256: f4442d079b22129199a62f5397106c7e623861bc226f80e8bf75d2a74907488f
translated_from: content/en/alg/VIII/A3_a3_hilbert_s_nullstellensatz.md
translation_method: google
source_content_sha256: 07f9a0ede5f4c5e394c02864754c6d680dbb4f9d6eb5a745c7ccb3b3fef1f87d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: a0edc8243f71be9fc99e76c7b1e4e26554cb989b20fe11eb83478922b7ed15ed
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 3 ヒルベルトヌルステレンザッツ

#### 定理 1 {#alg-viii-a3-thm-1 .statement tag=00QM}

A を整域、K を分数の体、L を可換K-代数とします。 A-代数 L が有限多数の元から生成され、L が体であるとします。

a) K 上の L の次数は有限です。

b) K が $A[a^{-1}]$ に等しいような A の非零元 $a$ が存在します。

S を A-代数 L の生成部分集合とします。私たちは S の基数に帰納法を用いるです。

まず、S の元がすべて K 上で代数的であるとします。K 上の L の次数は有限になります (V, §3, No. 2, p. 18, 定理 2)。 $(e_i)_{i\in I}$ を K 上の L の基底とします。A の非零元 $a$ が存在します。これに対する座標は、S の元の基底、元 1、および元 $e_ie_j$ です。 I 属するから $A[a^{-1}]$ の $i,j$。 線形結合 $\sum_{i\in I}a_ie_i$ の集合に、$i$ ごとに $a_i\in A[a^{-1}]$ を加えると、L の部分環になります。 含む A と S は構成なので、L と等しくなります。特に、含む $Ke_1$ であるため、K は $A[a^{-1}]$ に等しいです。

ここで、S の元 $s$ が K に対して超越的であるとします。 環 $A[s]$ の分数の E 体で表します。 $A[s$]-代数 L は S $-\{s\}$ によって生成されます。 帰納法の仮定までに、E が $A[s][P(s)^{-1}]$ に等しいような非零多項式 $P\in A[X]$ が存在します。 $\overline{K}$ を K の代数閉包とします (V, §4, No. 3, p. 23, 定理 2)。 体 $\overline{K}$ は無限 (V, §4, No. 1, p. 20, 命題 3) なので、$P(x)\not= 0$ となるような $\overline{K}$ のうち元 $x$ が存在します。 $\varphi : E\rightarrow K$ を K-代数 $E = A[s][P(s)^{-1}]$ から K-代数 $\overline{K}$ までの一意な準同型として、$s$ を $x$ に送信します。 E は K の超越論的拡大であり、$\overline{K}$ は K の代数的拡大であるため、これは不合理です。これで定理の証明が完成します。

#### 系 1 {#alg-viii-a3-thm-1-cor-1 .statement tag=00RV}

K を可換体、A を有限多数の元によって生成される可換K-代数、そして $\mathfrak{m}$ を A の最大理想とする。

a) K 上の $A/\mathfrak{m}$ の次数は有限です。

b) Ω を K の代数閉拡大とします。A から Ω まで核 $\mathfrak{m}$ で K-代数準同型が存在します。

K-代数 $A/\mathfrak{m}$ は有限多数の元から生成され、$A/\mathfrak{m}$ は体です。 定理 1 までに、$A/\mathfrak{m}$ の次数は有限です。 主張 a) が続きます。 有限次数の K のすべての拡大は Ω の部分拡張 (V, §4, No. 1、p. 20、定理 1) と同型です。これにより b) が得られます。

#### 系 2 {#alg-viii-a3-thm-1-cor-2 .statement tag=00QN}

K を可換体、$n$ を自然数、$(P_i)_{i\in I}$ を $K[X_1, . . . ,X_n]$ の元の族、Ω を K の代数閉拡大とします。次の条件は同等です。

(i) 多項式 $P_i$ には $\Omega^n$ に共通零点がありません。

(ii) $\sum_{i\in I}P_iQ_i= 1$ のような $K[X_1, . . . ,X_n]$ の元の有限台を持つ家族 $(Q_i)_{i\in I}$ が存在します。

A 環 $K[X_1, . . . ,X_n]$ と多項式 $P_i$ によって生成された理想を $\mathfrak{a}$ で表します。 条件 (i) は、$A/\mathfrak{a}$ から Ω までの K-代数準同型が存在しないことを意味します。それが満たされる場合、系 1 までに、環 $A/\mathfrak{a}$ には最大理想がないため、零、1 属するから $\mathfrak{a}$ になります。これは、(i) が (ii) を意味することを証明します。 (ii) $\Rightarrow$ (i) の含意は明らかです。
