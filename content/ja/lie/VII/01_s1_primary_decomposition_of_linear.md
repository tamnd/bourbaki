---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VII
chapter_title: CARTAN SUBALGEBRAS AND REGULAR ELEMENTS
section: 1
section_title: Primary decomposition of linear representations
lang: ja
source: lie-vii-ix
book_pages: 1-12, 51-55
pdf_pages: 0011-0022, 0060-0064
extraction: native
subsections:
    - "no": 1
      title: DECOMPOSITION OF A FAMILY OF ENDOMORPHISMS
      page: 1
      pdf_page: 11
    - "no": 2
      title: THE CASE OF A LINEAR FAMILY OF ENDOMORPHISMS
      page: 6
      pdf_page: 16
    - "no": 3
      title: DECOMPOSITION OF REPRESENTATIONS OF A NILPOTENT LIE ALGEBRA
      page: 8
      pdf_page: 18
    - "no": 4
      title: DECOMPOSITION OF A LIE ALGEBRA RELATIVE TO AN AUTOMORPHISM
      page: 11
      pdf_page: 21
    - "no": 5
      title: INVARIANTS OF A SEMI-SIMPLE LIE ALGEBRA RELATIVE TO A SEMI-SIMPLE ACTION
      page: 11
      pdf_page: 21
statements: 25
exercises: 11
content_sha256: 44d01d9cb5676562d930a25409f7ed8f21d468259b351992cc42491bef824dd4
translated_from: content/en/lie/VII/01_s1_primary_decomposition_of_linear.md
translation_method: google
source_content_sha256: 6d999a4f63ad71547f9729f56137320e39f7832c9c6c88d90de525d543eda5ce
translation_model: google-translate
translation_quality: low
translation_run: translate-ja-ca1d9542
glossary_version: 34
glossary_terms_sha256: aad8e0e2a7d603250a48c691491c8bf0ebc9e999d61e8dbad9c08bdebc6db211
prompt_sha256: 3ac95f6e208e19a9d7d5f609717955a23e34b6c1b333d157a4be9fc4e8dd1285
---

## § 1。一次的 分解/線型表現

### 1. 自己準同型人の家族の分解

VをSからエンド(V)までベクトル空間、Sを集合、$r$写像とします。 Sから$k$まで写像のP集合で表します。 $\lambda \in P$ の場合、すべての $s\in S,r(s)v=\lambda (s)v$ ($n$ 十分大きいの場合は $(r(s)-\lambda (s))^nv= 0$) について、$v\in V$ の $V_{\lambda}(S)$ (それぞれ $V^{\lambda}(S)$) 集合で表します。 集合 $V_{\lambda}(S)$ と $V^{\lambda}(S)$ は、V のベクトル部分空間と $V_{\lambda}(S)\subset V^{\lambda}(S)$ です。 $V_{\lambda}(S)$ は $\lambda$ (および $r$) に対する V の固有空間であり、$V^{\lambda}(S)$ は $\lambda$ (および $r$) に対する V の主部分空間であり、 $V^0(S)$ は、V ($r$ に対して) の無空間です。 $V^{\lambda}(S)\not= 0$なら、$\lambda$はVのSの重みであると言います。

特に、S 簡約するから単一の元 $s, P$ は $k$ で識別できます。 $V_{\lambda}(\{s\}), V^{\lambda}(\{s\})$ の代わりに、記法 $V_{\lambda(s)}(s)$ と $V^{\lambda(s)}(s)$、または $V_{\lambda(s)}(r(s))$ と $V^{\lambda(s)}(r(s))$ を使用します。私たちは固有空間、主部分空間とゼロ空間 $r(s)$ について話します。 $V_{\lambda(s)}(s)$ の元 $v$ は $r(s)$ の固有ベクトルと呼ばれ、$v\not= 0,\lambda (s)$ が対応する固有値と呼ばれます (cf. 代数、VII, §5 章)。

すべての $\lambda \in P$ に対して、次の関係は明らかです。

$$
V^{\lambda}(S) =\bigcap_{s\in S}V^{\lambda(s)}(s) \tag{1}
$$

$$
V_{\lambda}(S) =\bigcap_{s\in S}V_{\lambda(s)}(s) \tag{2}
$$

$k'$を$k$の拡大とします。 End(V) から End($V\otimes_kk'$) までの標準写像は、合成と $r$ により、写像 $r': S\rightarrow$ End($V\otimes_kk'$) になります。同様に、S から $k$ 定義するまでのすべての写像 $\lambda$ は、標準的には写像であり、S から $k'$ までの $\lambda$ でも表されます。これらの記法により、次の命題が得られます。

#### 命題 1 {#lie-vii-s1-prop-1 .statement tag=00SJ}

$\lambda \in P$の皆様、

$(V\otimes_kk')^{\lambda}(S) = V^{\lambda}(S)\otimes_kk'$と$(V\otimes_kk')_{\lambda}(S) = V_{\lambda}(S)\otimes_kk'$。

$(a_i)$ を $k$ ベクトル空間 $k'$ の基底とします。 $v\in V\otimes_kk',v$ が形 $\sum v_i\otimes a_i$ で一意に表現できる場合、$(v_i)$ は V の元の有限サポート族です。 $s\in S$の皆様、

$$
(r'(s)-\lambda (s))^n(v) =\sum(r(s)-\lambda (s))^nv_i\otimes a_i
$$

したがって、

$v\in (V\otimes_kk')^{\lambda}(S)\Leftarrow \Rightarrow v_i\in V^{\lambda}(S)$ 全員$i$、

すべての $i$ に対して $v\in (V\otimes_kk')_{\lambda}(S)\Leftarrow \Rightarrow v_i\in V_{\lambda}(S)$、

これは命題を意味します。

#### 命題 2 {#lie-vii-s1-prop-2 .statement tag=00SK}

$V,V',W$をベクトル空間とします。 $r$ : S $\rightarrow$ End(V)、$r': S\rightarrow$ End(V$'$)、$q: S\rightarrow$ End(W) を写像とします。

(i) $f: V\rightarrow W$ を、$s\in S$ と $v\in V$ に対して $q(s)f(v) =f(r(s)v)$ となるような線形写像とします。次に、すべての $\lambda \in P,f$ 写像 $V^{\lambda}(S)$ (それぞれ $V_{\lambda}(S)$) を $W^{\lambda}(S)$ (それぞれ $W_{\lambda}(S)$) にします。

(ii) $B : V\times V'\rightarrow W$ を次のような双線形写像とします。

$$
q(s)B(v, v') = B(r(s)v, v') + B(v, r'(s)v')
$$

$s\in S,v\in V,v'\in V'$の場合。次に、すべての $\lambda , \mu\in P$ について、B 写像 $V^{\lambda}(S)\times {V'}^\mu(S)$ (それぞれ $V_{\lambda}(S)\times V'_\mu(S)$) を $W^{\lambda+\mu}(S)$ (それぞれ $W_{\lambda+\mu}(S)$) に変換します。

(iii) $B : V\times V'\rightarrow W$ を次のような双線形写像とします。

$$
q(s)B(v, v') = B(r(s)v, r'(s)v')
$$

$s\in S,v\in V,v'\in V'$の場合。次に、すべての $\lambda , \mu\in P$ について、B 写像 $V^{\lambda}(S)\times {V'}^\mu(S)$ (それぞれ $V_{\lambda}(S)\times V'_\mu(S)$) を $W^{\lambda \mu}(S)$ (それぞれ $W_{\lambda \mu}(S)$) に変換します。

(i) の場合、$s\in S$ と $v\in V$ に対して $(q(s)-\lambda (s))^nf(v) =f((r(s)-\lambda (s))^nv)$ となるため、結論が得られます。 (ii)の場合、

$$
(q(s)-\lambda (s)-\mu(s))B(v, v') = B((r(s)-\lambda (s))v, v') + B(v,(r'(s)-\mu(s))v')
$$

$s\in S,v\in V,v'\in V'$ のため、したがって $n$ の帰納法まで

$$
'(n)''
$$

$(q(s)-\lambda (s)-\mu(s))^nB(v, v) =\sum B((r(s)-\lambda (s))^iv,(r(s)-\mu(s))^jv)$。

$$
i
$$

$i+j=n$

(ii)の主張はすぐに続きます。 (iii) の場合、$s\in S,v\in V,v'\in V'$ に対して $(q(s)-\lambda (s)\mu(s))B(v, v') = B((r(s)-\lambda (s))v, r'(s)v')+B(\lambda (s)v,(r'(s)-\mu(s))v')$、したがって $n$ には帰納法まで

$$
(q(s)-\lambda (s)\mu(s))^nB(v, v')
$$

= $\sum(n)B(\lambda (s)^j(r(s)-\lambda (s))^iv, r'(s)^i(r'(s)-\mu(s))^jv')$。

$$
i
$$

$i+j=n$

(iii) の主張はすぐに続きます。

#### 命題 3 {#lie-vii-s1-prop-3 .statement tag=00SL}

和 $\sum_{\lambda\in P}V^{\lambda}(S)$ は直接です。 和 $\sum_{\lambda\in P}V_{\lambda}(S)$ は直接です。

2 番目の主張は最初の帰結です。したがって、それを証明すれば十分です。いくつかのケースを区別します。

$a) S$は空いています。 主張は些細なことです。

$b) S$ は 1 つの元 $s$ に減ります。 $\lambda_0, \lambda_1, . . . , \lambda_n$ を $k$ の元と区別します。 $i= 0,1, . . . , n$ については、$v_i\in V^{\lambda_i}(s)$ とし、$v_0=v_1+\cdots +v_n$ と仮定します。 $v_0$ = 0 であることを証明すれば十分です。$i= 0, . . . , n$ の場合、$(r(s)-\lambda_i)^{q_i}v_i$ = 0 となる整数 $q_i>$ 0 が存在します。多項式 $P(X) =\prod_{i\geq 1}(X-\lambda_i)^{q_i}$ と $Q(X) = (X-\lambda_0)^{q_0}$ を考えてみましょう。 $Q(r(s))v_0= 0$ があり、

$P(r(s))v_0=\sum_{i=1}^nP(r(s))v_i= 0$。 P と Q は互いに素であるため、ベズー恒等式は $v_0= 0$ であることを証明します。

$c) S$ は有限で空ではありません。 S の基数について帰納法によって議論します。$s\in S$ と $S'= S$**--** $\{s\}$ とします。 $(v_{\lambda})_{\lambda\in P}$ を、$\sum_{\lambda\in P}v_{\lambda}= 0$ と $v_{\lambda}\in V^{\lambda}(S)$ のような V の元の有限支持家族とします。 $\lambda_0\in P$ にしましょう。 $P'$ を $\lambda \in P$ の集合として、$\lambda |S'=\lambda_0|S'$ とします。 帰納法の仮定を$S'$に適用すると、$\sum_{\lambda\in P'}v_{\lambda}= 0$になります。 $\lambda , \mu$ が $P',\lambda (s)\not=\mu(s)$ の元と異なる場合。

和 $\sum_{\alpha\in k}V^{\alpha}(s)$ は b) によって直接なので、$v_{\lambda}\in V^{\lambda(s)}(s),v_{\lambda}= 0$ 以降はすべての $\lambda \in P'$ 、特に $v_{\lambda_0}= 0$ について証明する必要がありました。

d) 一般的なケース。 $(v_{\lambda})_{\lambda\in P}$ を、$\sum_{\lambda\in P}v_{\lambda}= 0$ と $v_{\lambda}\in V^{\lambda}(S)$ のような V の元の有限支持族とします。 $P'$ を、$v_{\lambda}\not= 0$ となるような $\lambda \in P$ の有限集合とし、$S'$ を S の有限部分集合とし、条件 $\lambda \in P'$、$\mu\in P',\lambda |S'=\mu|S'$ は $\lambda =\mu$ を暗示します。 $v_{\lambda}\in V^{\lambda|S'}(S')$ があります。 適用 c)、$\lambda \in P'$ に対して $v_{\lambda}= 0$ が表示され、証明が完成します。

$x\in$ End(V) の場合、End(V) からそれ自体までの広告 $x$ 写像 $y \rightarrow xy-yx= [x, y]$ を表すことを思い出してください。

#### 補題 1 {#lie-vii-s1-lem-1 .statement tag=00SM}

$x, y\in$ 終了(V) にしましょう。

(i) V が有限次元であると仮定します。この場合、$x$ は $V =\sum_{a\in k}V^a(x)$ の場合にのみ三角形化可能です。

(ii) (ad $x$)$^ny= 0$ となるような整数 $n$ が存在する場合、各 $V^a(x)$ は $y$ の下で安定です。

(iii) V が有限次元であると仮定します。 $V =\sum_{a\in k}V^a(x)$ とそれぞれの場合

$V^a(x)$ は $y$ の下で安定しており、(ad $x$)$^ny= 0$ となる整数 $n$ が存在します。

部分 (i) は、代数章の続きです。 VII, §5, no. 2、提案 3。

E = 終了(V)とします。 B を $E\times V$ から V までの双線形写像 $(u, v) \rightarrow u(v)$ とします。広告 $x$ の定義までに、

$x(B(u, v)) =B(u, x(v)) +$ B((広告 $x$)$(u), v$)

$x\in E,u\in E,v\in V$の場合。 $x$ を広告 $x$ を介して E で操作します。提案 2 (ii) により、すべての $a\in k$ に対して $B(E^0(x),V^a(x))\subset V^a(x)$ が適用されます。 (ad $x$)$^ny= 0$ の場合、$y\in E^0(x)$、つまり $y(V^a(x))\subset V^a(x)$ となり、(ii) が証明されます。

(iii) を証明するには、$V^a(x)$ と $x$ (それぞれ $y$) の制限から $V^a(x)$ によって置き換える V ができます。 置き換えること $x$ $x-a$ により、$x$ はゼロポテントであると仮定できます。次に、(ad $x$)$^{2 dim V-1}= 0$ (Chap. I, §4, no. 2) となり、(iii) が証明されます。

#### 注意 {#lie-vii-s1-n1-rem-1 .statement tag=00SN}

この議論は、V が有限次元であり、(ad $x$)$^ny= 0$ となるような整数 $n$ が存在する場合、(ad $x$)$^{2 dim V-1}y= 0$ であることを証明します。

続編では、次の場合に写像 $r: S\rightarrow$ End(V) が条件 (AC) (「ほぼ可換」) を満たすと言うことにします。

(AC) S の元のすべての対 $(s, s')$ に対して、次のような整数 $n$ が存在します。

(広告$r(s)$)$^nr(s') = 0$。

#### 定理 1 {#lie-vii-s1-thm-1 .statement tag=00SO}

V が有限次元であると仮定します。次の条件は同等です。

(i) 条件 (AC) は満たされており、すべてにおいて $s\in S,r(s)$ は三角化可能です。

(ii) すべての $\lambda \in P$ について、$V^{\lambda}(S)$ は $r(S)$ および $V =\sum_{\lambda\in P}V^{\lambda}(S)$ の下で安定しています。

$V =\sum_{\lambda\in P}V^{\lambda}$(S) の場合、すべての $s\in S$ に対して $V =\sum_{a\in k}V^a(s)$ となり、次のようになります。

補題 1 (ii) は (i) を意味します。 条件 (i) が満たされると仮定します。 補題 1 と公式 (1) は、それぞれの $V^{\lambda}(S)$ が $r(S)$ の下で安定していることを意味します。 $V =\sum_{\lambda\in P}V^{\lambda}(S)$ を証明することはまだ残っています。私たちは薄暗いVで帰納法によって議論します。 2 つの場合を区別します。

a) すべての $s\in S,r(s)$ には 1 つの固有値 $\lambda (s)$ があります。続いて$V = V^{\lambda}(S)$。

b) $r(s)$ が少なくとも 2 つの異なる固有値を持つような $s\in S$ が存在します。すると、V は $a\in k$ の $V^a(s)$ の直和となり、すべての $a$ の$V^a(s)<$ V になります。各$V^a(s)$は$r$(S)以下で安定しており、帰納法の仮定を適用すれば十分です。

#### 系 1 {#lie-vii-s1-thm-1-cor-1 .statement tag=00SP}

V が有限次元であり、条件 (AC) が満たされると仮定します。 $k'$を$k$の拡大とします。すべての $s\in S$、$V\otimes_kk'$ の自己準同型 $r(s)\otimes 1$ が三角形化可能であると仮定します。 $P'$をSから$k'$までの写像の集合とします。それから$V\otimes_kk'=\sum_{\lambda'\in P'}(V\otimes_kk')^{\lambda'}(S)$。

$r': S\rightarrow$ End(V$\otimes_kk'$) を $r$ で定義される写像とします。 $s_1, s_2\in S$ の場合、(ad $r(s_1)$)$^nr(s_2) = 0$ となる整数 $n$ が存在するため、(ad $r'(s_1)$)$^nr'(s_2) = 0$ となります。ここで、Th を適用するだけで十分です。 1.

#### 系 2 {#lie-vii-s1-thm-1-cor-2 .statement tag=00SQ}

V が有限次元であり、条件 (AC) が満たされると仮定します。 $V^+(S)$ ベクトル部分空間 $\sum_{s\in S}((\bigcap_{i\geq 1}r(s)^iV)$ で表します。次に:

(i) $V^0(S)$ と $V^+(S)$ は $r(S)$ で安定しています。

(ii) $V = V^0(S)\oplus V^+(S)$;

(iii) V の各ベクトル部分空間 W は、$r(S)$ で安定しており、$W^0(S) = 0$ が $V^+(S)$ に含まれるようになります。

(iv) $\sum_{s\in S}r(s)V^+(S) = V^+(S)$。

さらに、$V^+(S)$ は、V の中で特性 (i) と (ii) を持つ唯一のベクトル部分空間です。 $k,(V\otimes_kk')^+(S) = V^+(S)\otimes_kk'$ のいずれかの拡大 $k'$ の場合。

最後の主張は明らかです。したがって、提案 1 を考慮すると、証明では他の提案では、$k$ が代数的に閉じていると仮定できます。 Thさんより1、V = $\sum_{\lambda\in P}V^{\lambda}$(S)、$V^{\lambda}(S)$ は $r(S)$ で安定します。 $s\in S$ の場合、特性

$r(s)|V^{\lambda}(S)$ の多項式は $(X-\lambda (s))^{dim V^{\lambda}(S)}$ です。つまり$\bigcap_{i\geq 1}r(s)^iV^{\lambda}(s)$

$\lambda (s) = 0$の場合は零、$\lambda (s)\not= 0$の場合は$V^{\lambda}(S)$に等しい。したがって、

$$
V^+(S) =\sum_{\lambda\in P,\lambda\not=0}V^{\lambda}(S) \tag{3}
$$

これは (i)、(ii)、(iv) を証明します。 W が $r$(S) で安定している V のベクトル部分空間であれば、$W =\sum_{\lambda\in P}W^{\lambda}(S)$ と $W^{\lambda}(S) = W\cap V^{\lambda}(S)$ になります。 $W^0(S) = 0$ の場合、$W\subset V^+$(S) がわかり、(iii) が証明されます。

$V'$ を $r(S)$ で安定し、$V'\cap V^0(S) = 0$ になるように V のベクトル部分空間とします。そうすると${V'}^0(S) = 0$なので、(iii)で$V'\subset V^+(S)$になります。 加法、$V = V^0(S) + V'$ では、$V'= V^+(S)$ であることがわかります。 Q.E.D.

ときどきは、V の $(V^0(S),V^+(S))$ フィッティング分解、または写像 $r: S\rightarrow$ End(V) を呼び出します。 S 簡約するを 1 つの元 $s$ に変換する場合、$V^+(\{s\})$ の代わりに $V^+(s)$ または $V^+(r(s))$ と書きます。 $V = V^0(s)\oplus V^+(s), V^0(s)$ と $V^+(s)$ は、$r(s),r(s)|V^0(s)$ がゼロポテントであり、$r(s)|V^+(s)$ が全単射である場合に安定であることがわかります。

#### 系 3 {#lie-vii-s1-thm-1-cor-3 .statement tag=00SR}

V と $V'$ を有限次元ベクトル空間とし、$r: S\rightarrow$ End(V) と $r': S\rightarrow$ End(V$'$) を写像満たす条件とします。 (AC)。 $f: V\rightarrow V'$ を、$s\in S$ と $v\in V$ に対して $f(r(s)v) =r'(s)f(v)$ となるような全射線形写像とします。次に、すべての $\lambda \in P$ に対して $f(V^{\lambda}{(S)) = V'}^{\lambda}(S)$ です。

提案 1 を考慮すると、$k$ が代数的に閉じている場合に帰着します。 Thの$V =\bigoplus_{\lambda\in P}V^{\lambda}$(S)、$V'=\bigoplus_{\lambda\in P}{V'}^{\lambda}(S)$がございます。 1、および $V'=f(V) =$ $\sum_{\lambda\in P}f(V^{\lambda}(S))$。最後に、提案 2 (i) により $f(V^{\lambda}(S))\subset {V'}^{\lambda}(S)$、よって系となります。

#### 命題 4 {#lie-vii-s1-prop-4 .statement tag=00SS}

$k$ が完璧であると仮定します。 V を End(V)$,u_s, u_n$ 半単純の有限次元ベクトル空間、$u$ 元と、$u($代数の零能成分とする。 VII, §5, no. 8）。

(i) $\lambda \in k,V^{\lambda}(u) = V^{\lambda}(u_s) = V_{\lambda}(u_s)$ 全員に対して。

(ii) V が代数構造で、$u$ が V$,u_s$ の導分で、$u_n$ が V の導分である場合。

(iii) V が代数構造で、$u$ が V の自己同型である場合、$u_s$ と $1 +u^{-1}_su_n$ は V の自己同型です。

提案 1 を考慮すると、$k$ は代数的に閉じていると仮定できます。

$$
V =\sum_{\lambda\in k}V^{\lambda}(u)
$$

$u|V^{\lambda}(u)$ の半単純成分は、$V^{\lambda}(u)$ の比率 $\lambda$ でホモテティー です。これは(i)を証明します。

これから、V に代数構造があるとします。 $x\in V^{\lambda}(u)$、$y\in V^\mu(u)$とします。

$u$ が V の導分である場合、$xy\in V^{\lambda+\mu}(u)$ (提案 2 (ii))、

$$
u_s(xy) = (\lambda +\mu)(xy) = (\lambda x)y+x(\mu y) = (u_sx)y+x(u_sy)
$$

これは、$u_s$がVの導分であることを証明します。すると$u_n=u-u_s$はVの導分です。

$u$ が V の自己同型である場合、Ker($u_s$) $= V^0(u) = 0$ なので、$u_s$ は全単射です。一方、$xy\in V^{\lambda \mu}(u)$（案2(iii)）なので、

$$
u_s(xy) = (\lambda \mu)(xy) = (\lambda x)(\mu y) =u_s(x).u_s(y)
$$

これは、$u_s$ が V の自己同型であることを証明します。でもそれもそうだ

$$
1 +u^{-1}_su_n=u^{-1}_su
$$

### 2. 自己準同型の直系家族の場合

ここで、S にはベクトル空間構造があり、写像 $r: S\rightarrow$ End(V) は線形であり、V と S は有限次元であると仮定します。

#### 命題 5 {#lie-vii-s1-prop-5 .statement tag=00ST}

条件 (AC) が満たされると仮定し、$\lambda : S\rightarrow k$ が $V^{\lambda}(S)\not= 0$ となるようにします。 $k$ が特性 0 の場合、写像 $\lambda$ は線形です。 $k$ が特性 $p\not= 0$ である場合、次元 $V^{\lambda}(S)$ を分割する $p$ の累乗 $q$ と、すべての $s\in S$ に対して $\lambda (s)^q= P(s)$ となる次数 $q$ の同次多項式関数 $P : S\rightarrow k$ が存在します。

$V^{\lambda}(S)$ は $r(S)$ (補題 1 と no. 1 の公式 (1)) の下で安定しているため、$V = V^{\lambda}(S)$ であると仮定できます。 $n=$ をV 暗くしましょう。したがって、$s\in S$ については、

デット(X $-r(s)$) $= (X-\lambda (s))^n$。

一方、行列式の展開は次のことを示しています。

デット(X $-r(s)$) $= X^n+a_1(s)X^{n-1}+\cdots +a_i(s)X^{n-i}+\cdots$

ここで、$a_i: S\rightarrow k$ は次数 $i$ の同次多項式関数です。 $k$と$(q, m) = 1$の特性指数の冪を$q$として$n=qm$と書きます。次に$(X-\lambda (s))^n= (X^q-\lambda (s)^q)^m$;したがって、$-m\lambda (s)^q=a_q(s)$ は結果を暗示します。

#### 命題 6 {#lie-vii-s1-prop-6 .statement tag=00SU}

$k$ が無限大で、条件 (AC) が満たされると仮定します。 $k'$ を $k$ の拡大とします。 $V'= V\otimes_kk',S'= S\otimes_kk'$を入れます。 $r': S'\rightarrow$ End(V$'$) を $r$ からスカラーの拡大で求めた写像とします。それから

$$
V^0(S)\otimes_kk'{= V'}^0{(S) = V'}^0(S')
$$

The first 等式 follows from Prop. 1. To prove the second, we can assume that $V = V^0(S)$ and so $V'{= V'}^0(S)$. Let $(s_1, . . . , s_m)$ be 基底 of S and $(e_1, . . . , e_n)$ 基底 of V.次のような多項式 $P_{ij}(X_1, . . . ,X_m)$ が存在します。

$$
r'(a_1s_1+\cdots +a_ms_m)^ne_j=\sum_{i=1}^nP_{ij}(a_1, . . . , a_m)e_i
$$

$1\leq j\leq n$ と $a_1, . . . , a_m\in k'$ の場合。 仮定、$r'(s)^n= 0$まではすべての$s\in S$に、その他の語$P_{ij}(a_1, . . . , a_m) = 0$は$1\leq i, j\leq n$と$a_1, . . . , a_m\in k$に。 $k$は無限大なので、$P_{ij}= 0$。従って、$r'(S')$ のすべての元は無能であり、$V'{= V'}^0(S')$ は無力です。

#### 命題 7 {#lie-vii-s1-prop-7 .statement tag=00SV}

$k$ が無限大であり、条件 (AC) が満たされると仮定します。 $\widetilde{S}$ を $s\in S$ の集合とし、$V^0(s) = V^0(S)$ とします。 $s\in S$ の場合、$P(s)$ を、$r(s)$ (no. 1、Th. 1 の Cor. 2 (i)) によって定義される $V/V^0(S)$ の自己準同型の行列式とします。

(i) 写像 $s \rightarrow P(s)$ は S 上の多項式です。$\widetilde{S} =\{s\in S|P(s)\not= 0\}$ があります。これはザリスキー 位相の S のオープン部分集合 (App. 1) です。

(ii) $\widetilde{S}$ は空ではなく、すべての $s\in \widetilde{S}$ に対して $V^+(s) = V^+(S)$ です。

$s \rightarrow P(s)$ が多項式であるという事実は、$r$ の線形性からわかります。 $s\in S, V^0(s)\supset V^0$(S) の場合、等式は、$V/V^0$(S) の $r(s)$ 定義する自己同型である場合に限り、(i) になります。

ここで、$k'$ を $k$ の代数閉包とし、提案 6 のように $V',S', r'$ を導入します。$S'$ は、$s_1, s_2\in S$ に対して有効な多項式恒等式 (ad $r(s_1)$)$^{2 dim V-1}r(s_2) = 0$ の継続によって条件 (AC) を満たすことに注目します。 (no. 1、注意 )。 適用 Th.1、私たちは分解と推測します

$$
V'{= V'}^0(S')\oplus \sum_{i=1}^m{V'}^{\lambda_i}(S')
$$

$\lambda_i\not= 0$ は $1\leq i\leq m$ です。 $1\leq i\leq m$ については、$S'$ と整数 $q_i$ にゼロ以外の多項式関数 $P_i$ が存在し、$\lambda^{q_i}_i= P_i$ となります (提案 5)。 $k$ は無限であるため、$(P_1. . .P_m)(s)\not= 0$, cf. 代数のような $s\in S$ が存在します。 IV, §2, no. 3、コル。提案 9 の 2。すると、すべての $i$ に対して $\lambda_i(s)\not= 0$、従って ${V'}^0(S'{) = V'}^0(s)$、その結果 $V^0(S) = V^0(s)$ (提案 6)、これは $\widetilde{S}\not=\emptyset$ を示します。 $s\in \widetilde{S}$ の場合、$V^+(S)$ が $r(s)$ で安定であり、V の $V^0(s)$ の補数であるという事実は、$V^+(S) = V^+(s)$ (Th. 1 の Cor. 2) を意味します。

### 3. 分解/表現/べき零リー代数

$\mathfrak{h}$ をリー代数とし、M を $\mathfrak{h}$ モジュールとします。 $\mathfrak{h}$ から $k$ までの任意の写像 $\lambda$ について、M の no. 1 ベクトル部分空間 $M^{\lambda}(\mathfrak{h})$ および $M_{\lambda}(\mathfrak{h})$ で定義しました。特に、$\mathfrak{g}$ がリー代数の場合、 含む $\mathfrak{h}$ を部分代数として、$x\in \mathfrak{g}$ の場合は、記法 $\mathfrak{g}^{\lambda}(\mathfrak{h})$ と $\mathfrak{g}_{\lambda}(\mathfrak{h})$ を使用することがよくあります。その場合、$\mathfrak{h}$ は$\mathfrak{g}$ に対して随伴表現 ad$_{\mathfrak{g}}$ によって作用することが理解されます。

#### 命題 8 {#lie-vii-s1-prop-8 .statement tag=00SW}

$\mathfrak{h}$ をリー代数とし、$L,M,N\mathfrak{h}$ モジュールとします。 $\mathfrak{h}$から$k$までの写像のP集合で表します。

(i) 和 $\sum_{\lambda\in P}L^{\lambda}(P)$ は直接です。

(ii) $f: L\rightarrow M$ が $\mathfrak{h}$ モジュールの準同型である場合、すべての $\lambda \in P$ に対して $f(L^{\lambda}(\mathfrak{h}))\subset M^{\lambda}(\mathfrak{h})$ になります。

(iii) $f: L\times M\rightarrow N$ が双一次 $\mathfrak{h}$ 不変量写像の場合、

$$
f(L^{\lambda}(\mathfrak{h})\times M^\mu(\mathfrak{h}))\subset N^{\lambda+\mu}(\mathfrak{h})
$$

$\lambda , \mu\in P$の皆さんへ。

これは Props からの続きです。 2と3。

#### 命題 9 {#lie-vii-s1-prop-9 .statement tag=00SX}

$\mathfrak{h}$ をべき零リー代数とし、M を有限次元の $\mathfrak{h}$ 加群とする。 $\mathfrak{h}$ から $k$ までは、写像の P 集合で表します。

(i) 各 $M^{\lambda}(\mathfrak{h})$ は M の $\mathfrak{h}$ サブモジュールです。$x_M$ がすべての $x\in \mathfrak{h}$ に対して三角化可能であれば、$M =\sum_{\lambda\in P}M^{\lambda}(\mathfrak{h})$ になります。

(ii) $k$ が無限大である場合、$M^0(x) = M^0(\mathfrak{h})$ となるような $x\in \mathfrak{h}$ が存在します。

(iii) $k$ が特性 0 で、$\lambda \in P$ が $M^{\lambda}(\mathfrak{h})\not= 0$ である場合、$\lambda$ は $\mathfrak{h}$ で線型形式となり、$[\mathfrak{h},\mathfrak{h}]$ で消滅し、$M_{\lambda}(\mathfrak{h})\not= 0$ になります。

(iv) $f: M\rightarrow N$ が有限次元 $\mathfrak{h}$ 加群の全射準同型である場合、すべての $\lambda \in P$ に対して $f(M^{\lambda}(\mathfrak{h})) = N^{\lambda}(\mathfrak{h})$ です。

(v) N が有限次元 $\mathfrak{h}$ 加群で、$\mathfrak{h}$ の下で $M\times N$ 上の B 双線形形式が​​$\lambda +\mu\not= 0$ であれば、$M^{\lambda}(\mathfrak{h})$ と $N^\mu(\mathfrak{h})$ は B に対して直交します。さらに、B が非縮退であれば、すべての $\lambda \in P$ の制限から $M^{\lambda}(\mathfrak{h})\times N^{-\lambda}(\mathfrak{h})$ も同様です。

部分 (i) は、no. 1、補題 1 および Th から続きます。 1. 部分 (ii) は、no. 2、提案 7 から導かれます。 部分 (iv) は、no. 1、Cor. 7 から導かれます。 Thの3。 1. (iii) を証明します。 $M = M^{\lambda}(\mathfrak{h})$ と仮定できます。次に、すべての $x\in \mathfrak{h},\lambda (x) =$ (薄暗い $M$)$^{-1}$Tr($x_M$);これは、$\lambda$ が線形であること (これも提案 5 から導かれる)、および $\lambda$ が $[\mathfrak{h},\mathfrak{h}]$ で消えることを証明します。によって定義された写像 $\rho :\mathfrak{h}\rightarrow$ End$_k(M)$ を検討してください。

$$
\rho (x) =x_M-\lambda (x)1_M
$$

上記より、これは M 上の $\mathfrak{h}$ の表現であり、$\rho (x)$ はすべての $x\in \mathfrak{h}$ に対して零です。エンゲルの定理 (第 1 章 I, §4, no. 2) によれば、M には $m\not= 0$ が存在し、すべての $x\in \mathfrak{h}$ に対して $\rho (x)m= 0$ となるため、$m\in M_{\lambda}(\mathfrak{h})$ になります。

(v) の最初の主張は、no. 1、提案 2 (ii) から続きます。 2 番目を証明するには、no. 1 の提案 1 を考慮して、$k$ が代数的に閉じていると仮定できます。次に、最初の事実と $M =\sum_{\lambda}M^{\lambda}(\mathfrak{h}), N =\sum_{\lambda}N^{\lambda}(\mathfrak{h})$, cf. (i) から続きます。

#### 注意 {#lie-vii-s1-n3-rem-1 .statement tag=00SY}

$k$ が完全で特性 2 であると仮定します。 $\mathfrak{h}=\mathfrak{s}\mathfrak{l}(2, k)$ とすると、

$$
_2(ab)
$$

M を $\mathfrak{h}$ モジュール $k$ とします ($\mathfrak{h}$ の単位写像の場合)。 $x=$ が

$$
ca
$$

$\mathfrak{h}$ の任意の元は、$\lambda^2=a^2+bc$ などの一意の $\lambda \in k$ を $\lambda (x)$ で示します。計算すると、$M = M^{\lambda}(\mathfrak{h})$ であることがすぐにわかります。一方、$M_{\lambda}(\mathfrak{h}) = 0$ と $\lambda$ は線形ではなく、$[\mathfrak{h},\mathfrak{h}]$ の零はなく、けれども $\mathfrak{h}$ でさえ零能です。

#### 系 {#lie-vii-s1-n3-cor-1 .statement tag=00SZ}

$\mathfrak{h}$ をべき零リー代数とし、M を $M^0(\mathfrak{h}) = 0$ のような有限次元 $\mathfrak{h}$ 加群とする。 $f:\mathfrak{h}\rightarrow M$ を次のような線形写像とします。

$x, y\in \mathfrak{h}$の場合は$f([x, y]) =x.f(y)-y.f(x)$。

すべての $x\in \mathfrak{h}$ に対して $f(x) =x.a$ となるような $a\in M$ が存在します。

$N = M\times k$ にしましょう。 $\mathfrak{h}$を公式によってNで演算させます

$$
x.(m, \lambda ) = (x.m-\lambda f(x),0)
$$

$f$ によって満たされる恒等式は、N が $\mathfrak{h}$ モジュールであることを意味します (章 I, §1, no. 8、例 2)。 N から $k$ への写像 $(m, \lambda ) \rightarrow \lambda$ は、N から自明な $\mathfrak{h}$ モジュール $k$ への準同型です。提案 9 (iv) により、形 $(a,1)$ と $a\in M$ の $N^0(\mathfrak{h})$ 含む元が得られます。 M の仮定を考慮すると、

$$
(M\times 0)\cap N^0(\mathfrak{h}) = 0
$$

したがって、$N^0(\mathfrak{h})$ は次元 1 であるため、$\mathfrak{h}$ によって消滅します。したがって、すべての $x\in \mathfrak{h}$ に対して $x.a-f(x) = 0$ となり、系が証明されます。

#### 命題 10 {#lie-vii-s1-prop-10 .statement tag=00T0}

$\mathfrak{g}$ をリー代数、$\mathfrak{h}$ を $\mathfrak{g}$ の nilpotent 部分代数とします。 $\mathfrak{h}$から$k$までの写像のP集合で表します。

(i) $\lambda , \mu\in P$、$[\mathfrak{g}^{\lambda}(\mathfrak{h}),\mathfrak{g}^\mu(\mathfrak{h})]\subset \mathfrak{g}^{\lambda+\mu}(\mathfrak{h})$ の場合。特に、$\mathfrak{g}^0(\mathfrak{h})$ は $\mathfrak{g}$ 含む $\mathfrak{h}$ の嘘部分代数であり、$\mathfrak{g}^{\lambda}(\mathfrak{h})$ は広告 $\mathfrak{g}^0(\mathfrak{h})$ の下で安定しています。さらに、$\mathfrak{g}^0(\mathfrak{h})$ は $\mathfrak{g}$ の独自のノーマライザーです。

(ii) M が $\mathfrak{g}$ モジュールの場合、$\lambda , \mu\in P$ に対して $\mathfrak{g}^{\lambda}(\mathfrak{h})M^\mu(\mathfrak{h})\subset M^{\lambda+\mu}(\mathfrak{h})$。特に、それぞれの $M^{\lambda}(\mathfrak{h})$ は $\mathfrak{g}^0(\mathfrak{h})$ モジュールです。

(iii) B が $\mathfrak{h},\mathfrak{g}^{\lambda}(\mathfrak{h})$ の下で不変である $\mathfrak{g}$ 上で双線形形式である場合、$\mathfrak{g}^\mu(\mathfrak{h})$ は $\lambda +\mu\not= 0$ に関して B に対して直交します。 B は非縮退であると仮定します。 次に、すべての $\lambda \in P$ について、B から $\mathfrak{g}^{\lambda}(\mathfrak{h})\times \mathfrak{g}^{-\lambda}(\mathfrak{h})$ までの制限は非縮退です。特に、B の制限から $\mathfrak{g}^0(\mathfrak{h})\times \mathfrak{g}^0(\mathfrak{h})$ は非縮退です。

(iv) $k$ が標数 0 であると仮定します。次に、$x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ と $\lambda \not= 0$ の場合、ad $x$ は零能です。

$\mathfrak{g}\times \mathfrak{g}$ から $\mathfrak{g}$ までの写像 $(x, y) \rightarrow [x, y]$ は、ヤコビ恒等式により $\mathfrak{g}$ 不変であるため、 $\mathfrak{h}$ 不変です。したがって、(i) の最初の部分は、提案 2 (ii) から導かれます。 部分 (ii) も同様に証明されます。

$\mathfrak{g}$ の $\mathfrak{g}^0(\mathfrak{h})$ のノーマライザーに $x$ 属するを適用すると、すべての $y\in \mathfrak{h}$ に対して (ad $y$)$.x=-[x, y]\in \mathfrak{g}^0(\mathfrak{h})$ となるため、$n$ 十分大きいに対して (ad $y$)$^n.x= 0$ となります。これは$x\in \mathfrak{g}^0(\mathfrak{h})$であることを証明します。 主張 (i) は完全に証明されました。

主張 (iii) は提案 9 (v) から導かれます。

(iv) を証明するには、$k$ が代数的に閉じていると仮定できます。 $x\in \mathfrak{g}^{\lambda}(\mathfrak{h})$ を $\lambda \not= 0$ にします。すべての $\mu\in P$ と任意の整数 $n\geq 0$ について、(ad $x$)$^n\mathfrak{g}^\mu(\mathfrak{h})\subset \mathfrak{g}^{\mu+n\lambda}(\mathfrak{h})$; $P_1$ を $\mathfrak{g}^\mu(\mathfrak{h})\not= 0$ となるような $\mu\in P$ の有限集合とします。 $k$ が特性 0 で、$n$ 十分大きいに対して $\lambda \not= 0, (P_1+n\lambda )\cap P_1=\emptyset$ の場合、(ad $x$)$^n= 0$ となります。

#### 補題 2 {#lie-vii-s1-lem-2 .statement tag=00T1}

$k$ が特性 0 であると仮定します。 $\mathfrak{g}$ を $k$ の半単純リー代数とします。B は、$\mathfrak{g},\mathfrak{m}$ の形 $\mathfrak{g}$ の部分代数です。次の条件が満たされていると仮定します。

1) B の制限から $\mathfrak{m}$ は非縮退です。

2) $\mathfrak{g}$ 属する ～ $\mathfrak{m}$ の $x\in \mathfrak{m}$、半単純および $x$ の無能成分$^1$ の場合。

すると、$\mathfrak{m}$は$\mathfrak{g}$で還元的になります（I, § 6, no. 6章）。

章著。 I, §6, no. 4、提案$5d),\mathfrak{m}$ は還元的です。 $\mathfrak{c}$を$\mathfrak{m}$の中心とします。 $x\in \mathfrak{c}$ が無能である場合、$x= 0$。実際、すべての $y\in \mathfrak{m}$、広告 $x$、および広告 $y$ の通勤について、それらの合成広告 $x\circ$ 広告 $y$ は零能であり、$B(x, y) = 0$ であるため、$x= 0$ です。ここで、$x$ を $\mathfrak{c}$ の任意の元とします。 $s$ と $n$ をその半単純と無能な成分とします。 $n\in \mathfrak{m}$があります。 ad $n$ は形 P(ad $x$) なので、P は定数のない多項式項、(ad $n$)$.\mathfrak{m}= 0$ となり、上記により $n\in \mathfrak{c}$、そして $n= 0$ となります。従って、広告 $x$ は半単純です。従って、$\mathfrak{g}$の随伴表現の制限から$\mathfrak{m}$は、半単純(章I, §6, no. 5、木$4b$)$)$となります。

#### 命題 11 {#lie-vii-s1-prop-11 .statement tag=00T2}

$k$ が標数 0 であると仮定します。 $\mathfrak{g}$ を半単純リー代数、$\mathfrak{h}$ を $\mathfrak{g}$ の冪能部分代数とします。 代数 $\mathfrak{g}^0(\mathfrak{h})$ は補題 2 の条件 (1) と (2) を満たします。 $\mathfrak{g}$ では還元的です。

$^1$ 章著I, §6, no. 3、木曜日。 3、すべての $x\in \mathfrak{g}$ は、相互に交換する半単純元 $s$ および冪零元 $n$ の和として一意に書くことができます。 元 $s$ (それぞれ $n$) は、$x$ の半単純 (それぞれ無能) 成分と呼ばれます。

$x, x'\in \mathfrak{g},s$ と $s'$ を、半単純成分、$n$、$n'$ を、それらの nilpotent 成分とします。我々は持っています

$x'\in \mathfrak{g}^0(x)\Leftarrow \Rightarrow$ (広告$s$)$(x') = 0$ (プロップ$.4$)

$\Leftarrow \Rightarrow$ (広告 $x'$)$(s) = 0$

$=\Rightarrow$ (広告 $s'$)$(s) = 0$

$\Leftarrow \Rightarrow$ (広告 $s$)$(s') = 0$

$\Leftarrow \Rightarrow s'\in \mathfrak{g}^0(x)$ (プロップ$.4$)

したがって、$x'\in \mathfrak{g}^0(x)\Rightarrow n'\in \mathfrak{g}^0(x)$ と (2) が証明されます。 $\mathfrak{g}$ の殺害形は非退化であるため、その制限から $\mathfrak{g}^0(\mathfrak{h})$ は非退化です (提案 10 (iii))。したがって、$\mathfrak{g}^0(\mathfrak{h})$ が $\mathfrak{g}$ で還元的であるという事実は、補題 2 から導かれます。

### 4. 自己同型に対するリー代数の分解

#### 命題 12 {#lie-vii-s1-prop-12 .statement tag=00T3}

$\mathfrak{g}$ を $\mathfrak{g}$ のリー代数、$a$ 自己同型とします。

(i) $\lambda , \mu\in k,[\mathfrak{g}^{\lambda}(a),\mathfrak{g}^\mu(a)]\subset \mathfrak{g}^{\lambda \mu}(a)$ の場合;特に、$\mathfrak{g}^1(a)$ は $\mathfrak{g}$ の部分代数です。

(ii) B が $a,\mathfrak{g}^{\lambda}(a)$ の下で $\mathfrak{g}$ 上の対称双線形形式であり、$\mathfrak{g}^\mu(a)$ が $\lambda \mu\not= 1$ に関して B に対して直交している場合。 B は非縮退であると仮定します。すると$\lambda \not= 0$、Bから$\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$の制限は非縮退です。

主張 (i) と (ii) の前半は、合成法則 $\mathfrak{g}\times \mathfrak{g}\rightarrow \mathfrak{g}$ および双線形形式 B に適用される提案 2 (iii) から導かれます。(ii) の後半を証明するには、$k$ が代数的に閉じていると仮定できます。次に$\mathfrak{g}=\bigoplus_{\nu\in k}\mathfrak{g}^{\nu}(a)$。上記を考慮すると、$\lambda \nu \not= 1$であれば$\mathfrak{g}^{\lambda}(a)$は$\mathfrak{g}^{\nu}(a)$と直交します。 B は非縮退であるため、その制限から $\mathfrak{g}^{\lambda}(a)\times \mathfrak{g}^{1/\lambda}(a)$ も同様であるということになります。

#### 系 {#lie-vii-s1-n4-cor-1 .statement tag=00T4}

$k$ が標数0 であり、$\mathfrak{g}$ が半単純であると仮定します。この場合、部分代数 $\mathfrak{g}^1(a)$ は補題 2 の条件 (1) と (2) を満たします。 $\mathfrak{g}$ では還元的です。

条件 (1) は提案 12 の部分 (ii) から導かれます。 条件 (2) は、no. 1 の提案 4 から続きます。

### 5. 半単純作用に対する半単純リー代数の不変量

この番号では$k$は標数0のものとします。

#### 命題 13 {#lie-vii-s1-prop-13 .statement tag=00T5}

$\mathfrak{g}$ を半単純リー代数、$\mathfrak{g}$ で $\mathfrak{g}$ の $\mathfrak{a}$ 部分代数、$\mathfrak{g}$ で $\mathfrak{a}$ の $\mathfrak{m}$ 交換子環とします。 部分代数 $\mathfrak{m}$ は、補題 2 の no. 3 の条件 (1) と (2) を満たします。 $\mathfrak{g}$ では還元的です。

第 6 章の提案による。 I, §3, no. 5、$\mathfrak{a}$ モジュール $\mathfrak{g}$ に適用すると、$\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$ になります。 B を $\mathfrak{g}$ の Killing 形とし、$x\in \mathfrak{a}, y\in \mathfrak{m}, z\in \mathfrak{g}$ とします。それから、

$B([z, x], y) = B(z,[x, y]) = 0$ $[x, y] = 0$ から、

これは、$\mathfrak{m}$ が B に対して$[\mathfrak{a},\mathfrak{g}]$ と直交していることを示しています。B は非縮退であり、$\mathfrak{g}=\mathfrak{m}\oplus [\mathfrak{a},\mathfrak{g}]$ なので、これは、B の制限から $\mathfrak{m}$ までが非縮退であることを意味します。したがって、補題 2 の条件 (1) は満たされます。

さて、$x\in \mathfrak{m}$ とし、$s$ と $n$ をその半単純とゼロポテント成分とします。広告$x$の半単純成分は広告$s$、cf.章です。 I, §6, no. 3。広告 $x$ は $\mathfrak{a}$ で零であるため、提案 4 (i) により、広告 $s$ も同様です。したがって、$s\in \mathfrak{m}$、したがって、$n=x-s\in \mathfrak{m}$、そして、補題 2 の条件 (2) が満たされます。

#### 注意 {#lie-vii-s1-n5-rem-1 .statement tag=00T6}

$\mathfrak{g}$ の $\mathfrak{m}$ の交換子環は、必ずしも簡約するから $\mathfrak{a}$、cf. を実行するとは限りません。 4.

#### 命題 14 {#lie-vii-s1-prop-14 .statement tag=00T7}

$\mathfrak{g}$を半単純リー代数、Aを群、$r$準同型をAからAut($\mathfrak{g}$)とします。 $\mathfrak{m}$ を $r(A)$ の下で不変である $\mathfrak{g}$ のからなるまたは元の部分代数とします。 線型表現 $r$ が半単純であると仮定します。すると、$\mathfrak{m}$ は条件 (1) と (2) の補題 2 の no. 3 を満たします。 $\mathfrak{g}$ では還元的です。

証明は、前述の命題と類似しています。

$\mathfrak{g}^+$ を、$r(a)x-x,a\in A, x\in \mathfrak{g}$ によって生成された $\mathfrak{g}$ のベクトル部分空間とします。 ベクトル空間 $\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$ は $r(A)$ 以下で安定しています。 $\mathfrak{n}$ を、$r(A)$ で安定した $\mathfrak{g}$ の $\mathfrak{g}'$ の補数とします。 $x\in \mathfrak{n}, a\in A,r(a)x-x\in \mathfrak{n}\cap \mathfrak{g}^+= 0$ の場合、$x\in \mathfrak{m}$ となり、$\mathfrak{m}\cap \mathfrak{n}= 0$ なので $x= 0$ となります。したがって、$\mathfrak{g}=\mathfrak{g}'=\mathfrak{m}+\mathfrak{g}^+$。 B を $\mathfrak{g}$ の殺害形とし、$y\in \mathfrak{m}, a\in A, x\in \mathfrak{g}$ とします。それから

$$
B(y, r(a)x-x) = B(y, r(a)x)-B(y, x)
$$

$$
= B(r(a^{-1})y, x)-B(y, x)
$$

$$
= B(y, x)-B(y, x) = 0
$$

したがって、$\mathfrak{m}$ と $\mathfrak{g}^+$ は B に対して直交します。したがって、B の制限から $\mathfrak{m}$ は非縮退であることがわかります。したがって、補題 2 の条件 (1) です。条件 (2) は、構造の輸送により明らかになります。

### 練習問題 {#lie-vii-s1-exercises}

それら上のすべてのリー代数と加群は、$k$ 上で有限次元であると想定されます。 §3以降、$k$は標数0のものとみなされます。

[§ 1 に対して練習問題](exercises/s1/)を参照してください。
