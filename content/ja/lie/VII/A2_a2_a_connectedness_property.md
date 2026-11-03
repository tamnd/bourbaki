---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 2
section_title: A connectedness property
appendix: true
lang: ja
source: lie-vii-ix
book_pages: 48-49, 67
pdf_pages: 0058-0059, 0076-0076
extraction: native
statements: 3
exercises: 2
content_sha256: 3c3af696db5888275392c7be4186bdc0bfa2da7476fd80536d372c14c8c370db
translated_from: content/en/lie/VII/A2_a2_a_connectedness_property.md
translation_method: google
source_content_sha256: e52c40721671251b25cbd21bd6c6376bf20e17aa16de77c1b806f74183e1c74a
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: aaf1806bbe58dc501429453a50818ba953a340244005c6718799716fd75974e9
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## 付録 II つながり性質

#### 補題 1 {#lie-vii-a2-lem-1 .statement tag=00XN}

X を接続されたトポロジー 空間とし、$\Omega$ を X の密で開いた部分集合とします。任意の $x\in X$ に対して、$V\cap \Omega$ が接続されるように $x$ の近傍 V が存在する場合、$\Omega$ が接続されます。

確かに、$\Omega_0$ を、$\Omega$ の空ではない開いた閉じた部分集合とします。 $x\in X$ と V を $x$ の近傍として、$V\cap \Omega$ が接続されるようにします。 $x\in \overline{\Omega}_0$の場合、

$$
(V\cap \Omega )\cap \Omega_0= V\cap \Omega_0\not=\emptyset
$$

だから$V\cap \Omega \subset \Omega_0$。従って、$X,\overline{\Omega}_0$では$\Omega$が密なので、$x$の近傍になります。従って、$\Omega_0$は空ではなく、開いていて閉じており、Xが接続されているため、$\overline{\Omega}_0= X$になります。 $\Omega_0$が$\Omega$で閉じているため、これは$\Omega_0=\Omega \cap \overline{\Omega}_0=\Omega$を意味し、$\Omega$が接続されていることを証明します。

#### 補題 2 {#lie-vii-a2-lem-2 .statement tag=00XO}

U を $\mathbf{C}^n$ と $f: U\rightarrow \mathbf{C}$ の正則写像であり、同一の零ではなく、オープン ボールであるとします。 A を A 上で $f= 0$ となるような U の部分集合とします。そのとき、U **--** A は U 内で密であり、連結。

U**--** A の稠密度は、微分可能と分析多様体、結果、3.2.5 から続きます。まず、$n= 1$ と仮定します。 $a\in A$, 冪系列 $a($微分可能および解析多様体についての $f$ の展開、結果、3.2.1) が 0 に減らされず、そのような U には $a$ の近傍 $V_a$ が存在することになります。 $f$ は $V_a$ **--** $\{a\}$ には消えません。従って、$a$ は A で孤立しており、これは A が U の離散部分集合であり、U が無限大で可算であるため可算であることを証明します。 $x, y\in U$ **--** A とします。A の $x$ (それぞれ $y$) と点を結ぶ実アフィン線の和集合はわずかです (一般位相、章 IX, §5, no. 2、定義 2)。従って、セグメント $[x, z]$ と $[y, z]$ のどちらも A と一致しないような $z\in U$ **--** A が存在します。 従って、点 $x, y, z$ は、U **--** A の同じ接続された成分に属するとなり、この場合、補題が証明されます。 $n= 1$。一般的なケースに移ります。 A は、$f($General 位相、Chap の集合の零であると仮定できます。 I, §11, no. 1、提案 1)。 $x, y\in U$**--** A とし、L をアフィン ライン含む $x$ と $y$ とします。 $f$ から $L\cap U$ の制限は、$x\in L\cap U$ 以降、零と同じではありません。すでに証明されていることから、$x$ と $y$ 属するは、$(L\cap U)$ **--** $(L\cap A)$ の同じ接続された成分に接続され、従って U **--** A の同じ接続された成分に接続されます。

#### 補題 3 {#lie-vii-a2-lem-3 .statement tag=00XP}

X を有限次元接続された複素解析多様体とし、A を次の条件 X 満たすの部分集合とします。

あらゆる $x\in X$ に対して、分析的な写像細菌 $f_x$ が存在し、消滅することはありません。

$x$ で、$x$ の A の胚芽が集合の $x$ の胚芽に含まれるようにします。

零の$f_x$。

すると、X **--** A は X に密集して接続されます。

X**--** A の稠密度は、微分可能と分析多様体、結果、3.2.5 から続きます。 A は閉じていると仮定できます (一般位相、章 I, §11, no. 1、提案 1)。任意の $x\in X$ については、V から $\mathbf{C}^n$ のオープン ボールまで、$x$ のオープン近傍 V と同型 $c$ が存在し、$c(A\cap V)$ が a の零の集合に含まれるようになります。正則写像は $c(V)$ の零と同じではありません。その後、補題 $2, V\cap (X$ **--** A) が接続されます。 補題 1 を考慮すると、これは X **--** A が接続されていることを証明します。

### 練習問題 {#lie-vii-a2-exercises}

[練習問題付録 2](exercises/a2/)を参照してください。
