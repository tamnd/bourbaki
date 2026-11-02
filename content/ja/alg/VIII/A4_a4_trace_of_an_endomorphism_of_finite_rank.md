---
book: alg
book_title: Algebra
chapter: VIII
chapter_title: Semisimple Modules and Rings
section: 4
section_title: Trace of an Endomorphism of Finite Rank
appendix: true
lang: ja
source: alg-viii
source_edition: 2023, Springer Nature
book_pages: A VIII.463-A VIII.467
pdf_pages: 0480-0484
extraction: native
subsections:
    - "no": 1
      title: Linear Mappings of Finite Rank
      page: 463
      pdf_page: 480
    - "no": 2
      title: Trace of an Endomorphism of Finite Rank
      page: 464
      pdf_page: 481
statements: 5
exercises: 2
content_sha256: 16346dab2041d5a923ddd48bd7fcbd2feff339ab7d57d4d22e0b5ee3261255fb
translated_from: content/en/alg/VIII/A4_a4_trace_of_an_endomorphism_of_finite_rank.md
translation_method: google
source_content_sha256: b21c8fa64810e183438c648b465f555368181eb6b34b8b9afdc829259a3d239d
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-b071ad41
glossary_version: 34
glossary_terms_sha256: c19645598a5de7cd9faa1cbf5c8b80e964072cafb33e0607dcb7fe6f84726e05
prompt_sha256: 08edf70d9b0078e74c7aa63f53b40428d18738541ef4c70faa747dfd1f79d030
---

## 付録 4 の自己準同型の有限階数のトレース

### 1. 有限階数中線形写像

Aを環、EとFをA-加群とします。 E から F までの線形写像の Hom$^f_A(E,F)$ 集合を、その像が F の有限生成された部分加群に含まれることを表します。それは Hom$_A(E,F)$ の部分群です。 Aが体のとき、有限階数のEからFまでは線形写像の集合です（II, §7, No. 4、p. 298、定義3）。 集合終わり$^f_A(E) =$ホム$^f_A(E,E)$。

$E,F,G$ を A-加群とし、$u: E\rightarrow F$ と $v: F\rightarrow G$ を A-線型写像とします。 $u\in$ Hom$^f_A(E,F)$ または $v\in$ Hom$^f_A(F,G)$ の場合、$v\circ u$ 属するから Hom$^f_A(E,G)$ となります。

$E^*\otimes_AF$ から Hom$_A(E,F)$ (II, §4, No. 2、p. 271) までの正規の群準同型を $\theta$ で表します。 $E^*\otimes_AF$ の元 $x^*\otimes y$ を E から F に写像 $x\mapsto  \langle x, x^*\rangle y$ に送信します。

#### 補題 1 {#alg-viii-a4-lem-1 .statement tag=00QO}

A-加群 F が射影であると仮定します。 群準同型 $\theta$ は単射であり、その像は Hom$^f_A(E,F)$ です。

ロケ地にて。前掲、系、準同型 $\theta$ は単射です。その像はHom$^f_A(E,F)$に含まれています。 $u\in$ ホム$^f_A(E,F)$ にしましょう。 $\theta$ の $u$ 属するから像であることを証明しましょう。

まず、A-加群 F がフリーであるとします。 $(f_i)_{i\in I}$ を F の基底とし、$(f_i^*)_{i\in I}$ を $F^*$ と $(f_i)_{i\in I}$ の双対の基底とします。 J を $j\in J$ の $f_j$ によって生成された F の部分加群に $u$ の像が含まれるように、I の有限部分集合とする。我々は持っています

$$
u(x) =\sum_{j\in J}\langle u(x), f_j^*\rangle f_j=\sum_{j\in J}\langle x,^tu(f_j^*)\rangle f_j \tag{1}
$$

$x\in E$ ごとに、したがって

$$
u=\theta (\sum_{j\in J}^tu(f_j^*)\otimes f_j) \tag{2}
$$

一般的なケースでは、$p\circ i= 1_F$ となるような自由A-加群 L と準同型 $i: F\rightarrow L$ と $p: L\rightarrow F$ が存在します。 準同型 $i\circ u$ 属するからホム$^f_A(E,L)$まで。上記により、有限の集合 J が存在し、各 $j\in J$ に対して、$E^*$ の元 $x^*_j$ と L の $y_j$ が存在します。

$$
i(u(x)) =\sum_{j\in J}\langle x, x^*_j\rangle y_j
$$

$x\in E$ごとに。次に、

$$
u(x) =p(i(u(x))) =\sum_{j\in J}\langle x, x^*_j\rangle p(y_j)
$$

$x\in E$ごとに、したがって$u=\theta (\sum_{j\in J}x^*_j\otimes p(y_j))$になります。

### 2. 有限階数の自己準同型の痕跡

この小節において、Aは可換環を表します。 E を射影 A-加群とします。 Then End$^f_A(E)$ is an A-submodule of End$_A$(E), and the canonical mapping $E^*\otimes_AE\rightarrow$ End$_A(E)$ defines an isomorphism $\theta_E$ of A-modules from $E^*\otimes_AE$ to End$^f_A(E)$ (Lemma 1). 公式 $\tau (x^*\otimes x) =\langle x, x^*\rangle$ によって特徴付けられる正規の線型形式 $\tau : E^*\otimes_AE\rightarrow A$ (II, §4, No. 3、p. 273) を考えてみましょう。 これを同型 $\theta^{-1}_E$ で合成すると、線型形式 Tr : End$^f_A(E)\rightarrow A$ が推定され、トレース形と呼ばれます。 A-加群 E が有限生成されると、II, §4, No. 3, p. 273 の定義が回収されます。

#### 命題 1 {#alg-viii-a4-prop-1 .statement tag=00QP}

E を自由A-加群とします。 $(e_i)_{i\in I}$ を E の基底とし、$(e^*_i)_{i\in I}$ をその双対基底とします。 $u\in$ を終了$^f_A(E)$ にしましょう。ファミリ $(\langle u(e_i), e^*_i\rangle )_{i\in I}$ には有限台があり、その和は Tr($u$) に等しいです。

$u$が形$\theta_E(x^*\otimes x)$の場合を$x\in E$と$x^*\in E^*$で扱えば十分です。家族 $(\langle x, e^*_i\rangle )_{i\in I}$ には有限台があり、私たちには $x=\sum_{i\in I}\langle x, e^*_i\rangle e_i$ がいます。従って、家族$(\langle x, e^*_i\rangle \langle e_i, x^*\rangle )_{i\in I}$には有限台もあり、私たちには$\langle x, x^*\rangle =\sum_{i\in I}\langle x, e^*_i\rangle \langle e_i, x^*\rangle$がいます。これで、$i\in I$ごとに$\langle u(e_i), e^*_i\rangle =\langle x, e^*_i\rangle \langle e_i, x^*\rangle$が得られます。これは命題を証明します。

#### 命題 2 {#alg-viii-a4-prop-2 .statement tag=00QQ}

E、F を射影 A-加群とします。 $u\in$ Hom$^f_A(E,F)$ と $v\in$ Hom$_A(F,E)$ とします。 関係あります

(3) トリ($v\circ u$) $=$ トリ($u\circ v$)。

$u$ が形 $\theta (x^*\otimes y)$ であるとき命題を $x^*\in E^*$ と $y\in F$ で証明すれば十分です。この場合、

$v\circ u=\theta_E(x^*\otimes v(y))$ と $u\circ v=\theta_F(^tv(x^*)\otimes y)$、

従って

トリ($v\circ u$) $=\langle v(y), x^*\rangle =\langle y,^tv(x^*)\rangle =$ トリ($u\circ v$)。

#### 系 {#alg-viii-a4-n2-cor-1 .statement tag=00QR}

E を射影 A-加群、$u$ を End$^f_A(E)$ の元、F を E 含む Im $u$ の射影 A-部分加群とします。 $u$ によって誘発された F の $u_F$ 自己準同型で表します。 我々は持っています

(4) トリ($u$) $=$ トリ($u_F$)。

F の $i$ 標準単射を E に、$u$ から推定した $v: E\rightarrow F$ 準同型で表します。 $u_F=v\circ i$と$u=i\circ v$があります。 系が続きます。

E を射影 A-加群および $u\in$ End$^f_A(E)$ とします。すべての自然数 $p$、A-加群 $\wedge^pE$ は射影 (III, §7, No. 8、p. 519、系 2)、および自己準同型 $\wedge^pu$ 属するから終わり$^f_A(\wedge^pE)$ までです。 (III, §7, No. 3、p. 511、命題 6)、$p$ 十分大きいの場合は零です。 集合 $1_E+$ エンド$^f_A(E)$ は合成以下で安定しています。私たちは定義する写像 $1_E+$ 終わり$^f_A(E)$ から設定までに A に到着します

det(1$_E+u$) $=\sum_{p\geqslant 0}$ Tr $\wedge^pu$

$u\in$ 終了$^f_A(E)$ 用。

If E is free and finite-dimensional, then this definition agrees with that of III, §8, No. 1, p. 522, by the corollary of III, §8, No. 5, p. 530.

#### 命題 3 {#alg-viii-a4-prop-3 .statement tag=00QS}

E を射影 A-加群とします。

a) $u\in$ を終了$^f_A(E)$ にします。 F を E 含む Im $u$ の射影 A-部分加群とし、$u_F$ を $u$ によって誘起される F の自己準同型とします。我々は持っています

(5) det(1$_E+u$) $=$ det(1$_F+u_F$)。

b) $u$ と $v$ を End$^f_A(E)$ の 2 つの元とします。我々は持っています

(6) det $(1_E+u)\circ (1_E+v)$ = det(1$_E+u$) det(1$_E+v$)。

a)を証明しましょう。 整数 $p\geqslant 0$ ごとに、射影 A-加群 $\wedge^pF$ は $\wedge^pE$ (III, §7, No. 9、p. 520、系) の部分加群と識別できます。 $\wedge^pu$の像は$\wedge^pF$に含まれており、$\wedge^pu$によって誘発された$\wedge^pF$の自己準同型は$\wedge^pu_F$に等しい。その結果、命題 2 の系によって Tr($\wedge^pu$) $=$ Tr($\wedge^pu_F$) が得られ、従って a) となります。

b)を証明しましょう。 G を A-加群として、A-加群 $L = E\oplus G$ が自由になるようにします。 L の $u'$ と $v'$ 自己準同型 $u\oplus 0_G$ と $v\oplus 0_G$ で表します。 a) により、関係 det(1$_L+u'$) $=$ det(1$_E+u$)、det(1$_L+v'$) $=$ det(1$_E+v$)、そして

デト(1$_L+u'+v'+u'\circ v'$) $=$ デト(1$_E+u+v+u\circ v$)。

したがって、A-加群 E が自由である場合、主張 b) を証明するだけで十分です。このとき、有限生成された自由な E の部分加群 F、$u$ の含む像と $v$ が存在します。 集合 $w=u+v+u\circ v$。 $w$の像はFに含まれており、$w_F=u_F+v_F+u_F\circ v_F$ができます。したがって、(5) により、det(1$_E+u$) $=$ det(1$_F+u_F$)、det(1$_E+v$) $=$ det(1$_F+v_F$) となります。

デット$((1_E+u)\circ (1_E+v))$

= det(1$_E+w$) $=$ det(1$_F+w_F$) $=$ det((1$_F+u_F$)$\circ (1_F+v_F)$)。

F は有限生成された自由A-加群であるため、次のようになります。

det((1$_F+u_F$)$\circ (1_F+v_F)$) $=$ det(1$_F+u_F$) det(1$_F+v_F$) $=$ det(1$_E+u$) det(1$_E+v$)。

### 練習問題 {#alg-viii-a4-exercises}

[練習問題付録 4](exercises/a4/)を参照してください。
