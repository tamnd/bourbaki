---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 1
section_title: The Lie algebra sl(2, k) and its representations
lang: zh
source: lie-vii-ix
book_pages: 69-77, 219-226
pdf_pages: 0077-0085, 0227-0234
extraction: native+ocr
subsections:
    - "no": 1
      title: CANONICAL BASIS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)
      page: 69
      pdf_page: 77
    - "no": 2
      title: PRIMITIVE ELEMENTS OF $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)-MODULES
      page: 70
      pdf_page: 78
    - "no": 3
      title: THE SIMPLE MODULES V($\boldsymbol{m}$)
      page: 72
      pdf_page: 80
    - "no": 4
      title: LINEAR REPRESENTATIONS OF THE GROUP SL(2$\boldsymbol{, k}$)
      page: 74
      pdf_page: 82
    - "no": 5
      title: SOME ELEMENTS OF SL(2$\boldsymbol{, k}$)
      page: 76
      pdf_page: 84
statements: 23
exercises: 18
content_sha256: 697f57b3381df1929231cecc5d02b74076b29a7e15f07931d667083d7f0df855
translated_from: content/en/lie/VIII/01_s1_the_lie_algebra_sl_2_k_and_its.md
translation_method: google
source_content_sha256: d56ad334c8b961365f3d72d7c521802edd95553bc6c867158ffa18290345692f
translation_model: google-translate
translation_quality: low
translation_run: translate-zh-0c690ed9
glossary_version: 34
glossary_terms_sha256: 7730eff5470fca5f9e58afb5e51b0372e5aaec572aa40387ee9f7593c4586e37
prompt_sha256: 31637ca47e680e9beb1f7812fc32fe615d0a63ad61fc456e4edc9253ad1563e9
---

## § 1。 李代数$\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)及其表示

### 1. 典范基 $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$)

#### 引理 1 {#lie-viii-s1-lem-1 .statement tag=00XS}

设 A 是 A 的 $k,H$ 和 $X$ 元素的结合律代数，使得 $[H, X] = 2X$。

(i) $[H, X^n] = 2nX^n$ 对于任何整数 $n\geq 0$。

(ii) 如果 $Z$ 是 A 的元素，使得 $[Z, X] =H$，则对于任意整数 $n >0$，

$$
[Z, X^n] =nX^{n-1}(H+n-1) =n(H-n+ 1)X^{n-1}
$$

从A到A的映射$T \rightarrow [H, T]$是推导，这意味着(i)。对于 (ii) 中的假设，

$$
[Z, X^n] =\sum_{i+j=n-1}X^iHX^j
$$

$$
=\sum_{i+j=n-1}(X^iX^jH+X^i2jX^j)
$$

$$
=nX^{n-1}H+ 2X^{n-1}\frac{n(n- 1)}{2}
$$

$$
=nX^{n-1}(H+n-1)
$$

另一方面，$X^{n-1}(H+n-1) = (H-n+ 1)X^{n-1}$乘以(i)。 Q.E.D.

回想一下，我们用阶 2 的方阵的 $\mathfrak{s}\mathfrak{l}(2, k)$ 李代数由……组成表示，跟踪零，并在 $k$ 中包含条目。这个李代数是维数3的简单组成（I, §6, no. 7，例）。 $\mathfrak{s}\mathfrak{l}(2, k)$ 的典范基是基 $(X_+, X_-, H)$，其中

$(01)($ 0 $0)(1$ 0 $)$

$X_+=$ 0 0 $X_-=-1$ 0 $H=$ 0 $-1$。

我们有

$$
[H, X_+] = 2X_+[H, X_-] =-2X_-[X_+, X_-] =-H \tag{1}
$$

由于$\mathfrak{s}\mathfrak{l}(2, k)$的恒等式表示是单射的，$H$是$\mathfrak{s}\mathfrak{l}(2, k)$的半单元素，$X_+, X_-$是$\mathfrak{s}\mathfrak{l}(2, k)$的幂零元（第I, §6, no. 3，第3章）。由章。 VII, §2, no. 1、例 $4,kH$ 是 $\mathfrak{s}\mathfrak{l}(2, k)$ 中的嘉当子代数。 映射$U \rightarrow  -^tU$是李代数$\mathfrak{s}\mathfrak{l}(2, k)$的对合自同构，称为$\mathfrak{s}\mathfrak{l}(2, k)$的规范对合；将变换$(X_+, X_-, H)$转换为$(X_-, X_+,-H)$。

#### 引理 2 {#lie-viii-s1-lem-2 .statement tag=00XT}

在$\mathfrak{s}\mathfrak{l}(2, k)$的包络线代数中，

$$
[H, X_+^n] = 2nX_+^n[H, X_-^n] =-2nX_-^n
$$

对于任意整数 $n\geq 0$，并且

$$
[X_-, X_+^n] =nX_+^{n-1}(H+n-1) =n(H-n+ 1)X_+^{n-1}
$$

$$
[X_+, X_-^n] =nX_-^{n-1}(-H+n-1) =n(-H-n+ 1)X_-^{n-1}
$$

如果$n >0$。

第一个和第三个关系源自引理1。其他的可以通过使用$\mathfrak{s}\mathfrak{l}(2, k)$的规范对合从它们中推出。

### 2. $\mathfrak{s}\mathfrak{l}$(2$\boldsymbol{, k}$) 的原语元素-模块

令 E 为 $\mathfrak{s}\mathfrak{l}(2, k$) 模。如果$A\in \mathfrak{s}\mathfrak{l}(2, k)$和$x\in E$，我们通常会写$Ax$而不是$A_Ex$。让$\lambda \in k$。如果$Hx=\lambda x$我们滥用语言，$x$是权$\lambda$的E的元素，或者$\lambda$是$x$的权。如果E是有限维的，$H_E$是半单，那么权$\lambda$的元素的集合是E相对于$H_E$和$\lambda$的主子空间（cf.） VII, §1, no. 1）。

#### 引理 3 {#lie-viii-s1-lem-3 .statement tag=00XU}

如果$x$是权$\lambda$中的元素，则$X_+x$是权$\lambda + 2$中的元素，$X_-x$是权中的元素 $\lambda -2$。

事实上，$HX_+x= [H, X_+]x+X_+Hx= 2X_+x+X_+\lambda x= (\lambda + 2)X_+x$，类似的$HX_-x= (\lambda -2)X_-x$（cf.也是第VII, §1, no. 3章，提案10（ii））。

#### 定义 1 {#lie-viii-s1-def-1 .statement tag=00XV}

令 E 为 $\mathfrak{s}\mathfrak{l}(2, k)$ 模。如果E的元素是$H_E$和属于到$X_{+E}$的核的非零特征向量，则称它是本原的。

E 的非零元素 $e$ 是原语当且仅当 $ke$ 在运算的 $kH+kX_+$ 下稳定；这是从引理 3 开始的例。

例元素 $X_+$ 是$\mathfrak{s}\mathfrak{l}(2, k)$ 的伴随表示的权 2 的原语。对于$k^2$上$\mathfrak{s}\mathfrak{l}(2, k)$的恒等式表示，$k^2$的元素$(1,0)$是权1的原语。

#### 引理 4 {#lie-viii-s1-lem-4 .statement tag=00XW}

令 E 为非零有限维 $\mathfrak{s}\mathfrak{l}(2, k)$ 模。那么 E 有原语元素。

由于$X_+$是幂零元，$\mathfrak{s}\mathfrak{l}(2, k),X_{+E}$是幂零的。假设 $X_{+E}^{m-1}\not= 0$ 和 $X_{+E}^m$ = 0。通过引理 2，

$$
m(H_E-m+ 1)X_{+E}^{m-1}= [X_{-E}, X_{+E}^m] = 0
$$

因此 $X_+^{m-1}(E)$**--** $\{0\}$ 的元素是原始的。

#### 命题 1 {#lie-viii-s1-prop-1 .statement tag=00XX}

令 E 为 $\mathfrak{s}\mathfrak{l}(2, k)$ 模，$e$ 权 $\lambda$ 的 E 的原语元素。将 $e_n=\frac{(-1)^n}{n}X_-^ne$ 替换为 $n\geq 0$，以及 $e_{-1}= 0$。然后

$$
He_n= (\lambda -2n)e_n
$$

$$
X_-e_n=-(n+ 1)e_{n+1} \tag{2}
$$

$$
X_+e_n= (\lambda -n+ 1)e_{n-1}
$$

第一个公式来自引理3，第二个定义来自$e_n$。我们通过$n$上的归纳证明了第三个。从$e_{-1}= 0$开始$n= 0$就满足了。如果$n >0$，

$$
nX_+e_n=-X_+X_-e_{n-1}=-[X_+, X_-]e_{n-1}-X_-X_+e_{n-1}
$$

$$
=He_{n-1}-X_-(\lambda -n+ 2)e_{n-2}
$$

$$
= (\lambda -2n+ 2 + (n-1)(\lambda -n+ 2))e_{n-1}
$$

$$
=n(\lambda -n+ 1)e_{n-1}
$$

#### 推论{#lie-viii-s1-n2-cor-1 .statement tag=00XY}

$e$生成的E的子模是$e_n$生成的向量子空间。

这是从公式 (2) 得出的。

整数$n\geq 0$，使得$e_n\not= 0$构成$\mathbf{N}$中的一个区间，并且$e$生成的子模的$k$上有相应的元素$e_n$形式基 （事实上，它们是线性独立的，因为它们是不同的权的非零元素）。这个基将被认为与原语元素$e$相关联。

#### 命题 2 {#lie-viii-s1-prop-2 .statement tag=00XZ}

如果由原语元素$e$生成的E的子模V是有限维的，则：

(i) $e$ 的权 $\lambda$ 是整数且等于 dim $V-1$；

(ii) $(e_0, e_1, . . . , e_{\lambda})$是V中的基，$e_n= 0$是$n > \lambda$；

(iii) $H_V$中的特征值为$\lambda , \lambda -2, \lambda -4, . . . ,-\lambda$；它们都是重数 1；

(iv) V 的每个原语元素都与 $e$ 成比例；

(v) 模 V 的交换子被约化为标量；特别是V绝对简单。

令$m$为最大的整数，使得$e_m\not= 0$。然后$0 =X_+e_{m+1}=$$(\lambda -m)e_m$，所以$\lambda =m$；由于$(e_0, e_1, . . . , e_m)$是V的基，这证明了(i)和(ii)。 断言 (iii) 源自等式 $He_n= (\lambda -2n)e_n$。我们有 $X_+e_n\not= 0$ 对应 $1\leq n\leq m$，因此 (iv)。设$c$为模V的交换子元素。那么$Hc(e) =cH(e) =\lambda c(e)$，所以存在$\mu\in k$使得$c(e) =\mu e$；然后

$$
cX_-^qe=X_-^qce=\mu X_-^qe
$$

对于所有 $q\geq 0$，因此 $c=\mu.1$，证明 (v)。

#### 推论{#lie-viii-s1-n2-cor-2 .statement tag=00Y0}

令 E 为有限维 $\mathfrak{s}\mathfrak{l}(2, k)$ 模。

(i) 自同态 $H_E$ 可对角化的，并且其特征值是有理数整数。

(ii) 对于任何$p\in \mathbf{Z}$，令$E_p$为$H_E$相应的到特征值$p$的特征空间。令$i$为整数$\geq 0$。 映射 $X_{-E}^i|E_p: E_p\rightarrow E_{p-2i}$ 是 $i\leq p$ 的单射，$i=p$ 的双射，$i\geq p$ 的满射。 映射 $X_{+E}^i|E_{-p}: E_{-p}\rightarrow E_{-p+2i}$ 是 $i\leq p$ 的单射，$i=p$ 的双射，$i\geq p$ 的满射。

(iii) E 的长度等于dim Ker$X_{+E}$和dim Ker$X_{-E}$。

(iv) 对于$p$偶数（或奇数），令$E'$（或$E''$）为$E_p$的和。则$E'$（或$E''$）为奇数（或偶数）维数 E 简单子模和；和$E = E'\oplus E''$。 $E'$的长度暗淡$E_0$，$E''$的暗淡$E_1$。

(v) Ker$X_{+E}\cap$ Im$X_{+E}\subset \sum_{p>0}E_p$ 和 Ker$X_{-E}\cap$ Im$X_{-E}\subset \sum_{p<0}E_p$。

如果 E 很简单，则 E 由原语元素 (引理 4) 生成，并且满足应用命题 1 和 2。 一般情况如下，因为每个有限维 $\mathfrak{s}\mathfrak{l}(2, k$) 模都是半单。

### 3.单模V($\boldsymbol{m}$)

设$(u, v)$为$k^2$的典范基。对于$\mathfrak{s}\mathfrak{l}(2, k)$的恒等式表示，

$$
X_+u= 0Hu=uX_-u=-v
$$

$$
X_+v=uHv=-vX_-v= 0
$$

考虑 $k^2($代数的对称代数 $\mathbf{S}(k^2)$，第 1 章。 III, §6, no. 1，默认。 1）。 $\mathfrak{s}\mathfrak{l}(2, k)$ 扩展的元素与 $\mathbf{S}(k^2)$ 的推导唯一，给出 $\mathfrak{s}\mathfrak{l}(2, k$) 模的 $\mathbf{S}(k^2)$ 结构（第 1 章） I, §3, no. 2）。 Let $V(m)$ be the set of homogeneous elements of $\mathbf{S}(k^2)$ of degree $m$. 那么$V(m)$是维数$m+ 1$的$\mathbf{S}(k^2)$的$\mathfrak{s}\mathfrak{l}(2, k$)子模，$V(1) =k^2$的第$m$对称幂（第1章） III，附录）。 如果 $m, n$ 是整数使得 $0\leq n\leq m$，则将

$$
e^{(m)}_n=(m)u^{m-n}v^n\in V(m)
$$

$$
n
$$

#### 命题 3 {#lie-viii-s1-prop-3 .statement tag=00Y1}

对于任何整数$m\geq 0$，$V(m)$是一个绝对简单的$\mathfrak{s}\mathfrak{l}(2, k)$模块。在这个模中，$e^{(m)}_0=u^m$是权$m$的原语。

我们有$X_+u^m= 0$和$Hu^m=mu^m$，所以$u^m$是权$m$的原语。由$u^m$生成的$V(m)$的子模是维数$m+ 1$（命题2（i）），因此等于$V(m)$。根据命题 2 (v)，$V(m)$ 绝对简单。

#### 定理 1 {#lie-viii-s1-thm-1 .statement tag=00Y2}

有限维 $n$ 的每个简单$\mathfrak{s}\mathfrak{l}(2, k)$模都与$V(n-1)$同构的。每个有限维$\mathfrak{s}\mathfrak{l}(2, k)$模都是子模的直和同构于模$V(m)$。

这是从引理 4 和命题 1、2 和 3 得出的。

#### 注 1 {#lie-viii-s1-n3-rem-1 .statement tag=00Y3}

简单 $\mathfrak{s}\mathfrak{l}(2, k$) 模的$\mathfrak{s}\mathfrak{l}(2, k)$ 结构上$\mathfrak{s}\mathfrak{l}(2, k)$ 定义的伴随表示。这个模通过同构与V(2)同构的，需要$u^2$到$X_+, 2uv$到$-H$，以及$v^2$到$X_-$。

#### 注 2 {#lie-viii-s1-n3-rem-2 .statement tag=00Y4}

对于 $n\geq 0$ 和 $m > n$，

$$
X_-e^{(m)}_n=-(m-n)(m)u^{m-n-1}v^{n+1}=-(n+ 1)e^{(m)}_{n+1}
$$

$$
n
$$

因此，$(e_0^{(m)}, e_1^{(m)}, . . . , e_m^{(m)})$ 是与原语元素 $e_0^{(m)}$ 伴随的 $V(m)$ 的基。

#### 注 3 {#lie-viii-s1-n3-rem-3 .statement tag=00Y5}

令 $\Phi$ 为 $V(m)$ 上的双线性形式，使得

$\Phi (e^{(m)}_n, e^{(m)}_{n'}) = 0$如果$n+n'\not=m$

$$
\Phi (e^{(m)}_n, e^{(m)}_{m-n}) = (-1)^n(m)
$$

$$
n
$$

如果$x=au+bv$和$y=cu+dv$，则$\Phi (x^m, y^m) = (ad-bc)^m$。现在很容易检查$\Phi$是不变的，并且$\Phi$对于$m$偶数是对称的，交错的对于$m$奇数是对称的。

#### 命题 4 {#lie-viii-s1-prop-4 .statement tag=00Y6}

设E是权$m$的原语元素的有限维$\mathfrak{s}\mathfrak{l}(2, k)$模、$m$整数$\geq 0$、$P_m$集合。令L为从$\mathfrak{s}\mathfrak{l}(2, k)$模$V(m)$到$\mathfrak{s}\mathfrak{l}(2, k)$模E的同态的向量空间。从L到E的映射$f \rightarrow f(u^m)$是线性、单射的，其像为$P_m\cup  \{0\}$。

这个映射显然是线性的，并且它是单射的，因为 $u^m$ 生成 $\mathfrak{s}\mathfrak{l}(2, k$)-模 $V(m)$。如果$f\in L$，

$$
X_+(f(u^m)) =f(X_+u^m) = 0,H(f(u^m)) =f(Hu^m) =mf(u^m)
$$

所以$f(u^m)\in P_m\cup  \{0\}$。设$e\in P_m$，以及$e$生成的E的V子模。根据命题1，存在从模$V(m)$到模V的同构，需要$u^m$到$e$。然后$L(u^m) = P_m\cup  \{0\}$。

#### 推论{#lie-viii-s1-n3-cor-1 .statement tag=00Y7}

型 $V(m)$ 的 E 的同型成分有长度

昏暗(P$_m\cup  \{0\}$.

### 4. 特殊线性群(2$\boldsymbol{, k}$)中的线性表示

回想一下（代数，III, §8, no. 9），我们用阶 2 的方阵的 $\mathbf{S}\mathbf{L}(2, k)$ 群表示，$k$ 中的系数其行列式等于 1。如果 $x\in \mathfrak{s}\mathfrak{l}(2, k)$ 幂零的，则$x^2= 0 ($代数，第 1 章VII, §5，科。提案 5 中的 3) 和 $e^x= 1 +x\in \mathbf{S}\mathbf{L}(2, k)$。如果 E 是有限维向量空间并且 $\rho$ 是 E 上 $\mathfrak{s}\mathfrak{l}(2, k)$ 的线性表示，则 $\rho (x)$ 幂零的，因此定义 $e^{\rho(x)}$（第 I, §6, no. 3 章）。

#### 定义 2 {#lie-viii-s1-def-2 .statement tag=00Y8}

设 E 为有限维向量空间，并且 E 上的 $\mathfrak{s}\mathfrak{l}(2, k)$（分别为 $\mathbf{S}\mathbf{L}(2, k)$）的 $\rho$（分别为 $\pi$）线性表示。则 $\rho$ 和 $\pi$ 被认为是兼容的，如果对于每个幂零元 $x$ $\mathfrak{s}\mathfrak{l}(2, k),\pi (e^x) =e^{\rho(x)}$。

在其他字，$\rho$和$\pi$是兼容的，如果对于$\mathfrak{s}\mathfrak{l}(2, k)$的每个幂零元$x$，$\rho$到$kx$的限制与$\pi$到限制兼容群$1 +kx$（第VII, §3, no. 1章）。

如果$\rho$和$\pi$相容的，那么对偶表示、$m$第张量幂以及$\rho$和$\pi$的第$m$对称幂也分别兼容（第1章）。 VII, §5, no. 4、引理 1 (i) 和 (ii))。 同样，对于$\rho$和$\pi$在向量子空间上诱导的表示在$\rho$和$\pi ($loc下稳定。引用。）。

特别是，$V(m)$（no. 3）上$\mathfrak{s}\mathfrak{l}(2, k)$的表示$\rho_m$与$\mathbf{S}\mathbf{L}(2, k)$的恒等式表示$\pi_1$的第$m$对称幂$\pi_m$相容的。将$e^{(m)}_n=(^m_n)u^{m-n}v^n$如上所示，我们有

$(m)(m)m-nn$

$\pi_m(s)e_n$ = $(su)(sv)$ (3)

$$
n
$$

对于 $s\in \mathbf{S}\mathbf{L}(2, k)$ 和 $0\leq n\leq m$。

#### 定理 2 {#lie-viii-s1-thm-2 .statement tag=00Y9}

令 $\rho$ 为 $\mathfrak{s}\mathfrak{l}(2, k)$ 在有限维向量空间 E 上的线性表示。

(i) E 上存在与 $\rho$ 兼容的唯一 $\mathbf{S}\mathbf{L}(2, k)$ 线性表示 $\pi$。

(ii) E 的向量子空间 F 在 $\pi$ 下稳定当且仅当它在 $\rho$ 下稳定。

(iii)设$x\in E$。那么$\pi (s)x=x$对于所有$s\in \mathbf{S}\mathbf{L}(2, k)$当且仅当$x$在$\rho ($下不变，即$\rho (a)x= 0$对于所有$a\in \mathfrak{s}\mathfrak{l}(2, k))$。

$\pi$ 的存在由前面的 和 Th 推出。 1. 另一方面，我们知道群$\mathbf{S}\mathbf{L}(2, k)$是由形式的元素生成的

$$
_{tX}(1t)_{-tX_-}(10)
$$

$e^+=e$ =

0 1 $t$ 1

其中 $t\in k($代数，第 1 章III, §8, no. 9，提案 17）。这就证明了$\pi$的唯一性。

断言 (ii) 和 (iii) 遵循我们与第 1 章所说的内容。 VII, §3, no. 1、引理 1 (i)。 Q.E.D.

因此，每个有限维 $\mathfrak{s}\mathfrak{l}(2, k$) 模块都有一个独特的 $\mathbf{S}\mathbf{L}(2, k)$ 模块结构，据说与其 $\mathfrak{s}\mathfrak{l}(2, k$) 模块结构相关。

#### 注 {#lie-viii-s1-n4-rem-1 .statement tag=00YA}

当$k$为$\mathbf{R}$或$\mathbf{C}$或完全非离散超度量域时，$\mathfrak{s}\mathfrak{l}(2, k)$为$\mathbf{S}\mathbf{L}(2, k)$的李代数。令 $\rho$ 和 $\pi$ 如 Th 中所示。 2. 同态$\pi$是李群从$\mathbf{S}\mathbf{L}(2, k)$到$\mathbf{G}\mathbf{L}(E):$的同态，这在$E = V(m)$时是清楚的，一般情况如下，鉴于Th。 1. 章。 VII, §3，没有。 $1,\rho (X_+) = L(\pi )(X_+),\rho (X_-) = L(\pi )(X_-)$。因此$\rho = L(\pi )$（对于逆命题，参见练习18）。

#### 命题 5 {#lie-viii-s1-prop-5 .statement tag=00YB}

令 E、F 为有限维 $\mathfrak{s}\mathfrak{l}(2, k)$ 模，并令 $f\in$ Hom$_k(E,F)$。以下条件是等效的：

(i) $f$ 是 $\mathfrak{s}\mathfrak{l}(2, k)$ 模块中的同态；

(ii) $f$ 是 $\mathbf{S}\mathbf{L}(2, k)$ 模块中的同态。

条件 (i) 表示 $f$ 是 $\mathfrak{s}\mathfrak{l}(2, k$) 模块 Hom$_k(E,F)$ 的不变量元素，条件 (ii) 表示 $f$ 是 $\mathbf{S}\mathbf{L}(2, k$) 模块的不变量元素坎$_k(E,F)$。由于这些模结构与第 1 章相关联。 VII, §5, no. 4、引理 1 (iii)、命题由 Th 得出。 2（三）。

#### 定义 3 {#lie-viii-s1-def-3 .statement tag=00YC}

群 $\mathbf{S}\mathbf{L}(2, k)$ 的伴随表示是 $\mathbf{S}\mathbf{L}(2, k)$ 在 $\mathfrak{s}\mathfrak{l}(2, k)$ 上的线性表示 Ad 定义为

广告($s$)$.a=sas^{-1}$

对于所有 $a\in \mathfrak{s}\mathfrak{l}(2, k)$ 和所有 $s\in \mathbf{S}\mathbf{L}(2, k)$。当$k$是$\mathbf{R}$或$\mathbf{C}$或完全非离散超度量域时，我们恢复Def。第 7 章III, §3, no. 12（cf.，参见第 49 号提案）。

由章。 VII, §5, no. 4、引理 1 (i) 和 (ii)、$\mathfrak{s}\mathfrak{l}(2, k)$ 和$\mathbf{S}\mathbf{L}(2, k)$ 的伴随表示是兼容的。由章。 VII, §3, no. 1、注2、广告($\mathbf{S}\mathbf{L}(2, k)$)$=$自动$_e(\mathfrak{s}\mathfrak{l}(2, k))$。

### 5. 一些元素 SL(2$\boldsymbol{, k}$)

对于任意 $t\in k^*$，将

$$
\theta (t) =e^{tX_+}e^{t^{-1}X_-}e^{tX_+}
$$

$(1t)(($ 1 $0)((1t)$

= 0 1 $-t^{-1}$ 1 0 1

$($0吨)

=$-t^{-1}$0

$$
=e^{t^{-1}X_-}e^{tX_+}e^{t^{-1}X_-}
$$

记号 no. 3，

$$
\theta (t)u=-t^{-1}v\theta (t)v=tu
$$

所以

$$
\theta (t)e^{(m)}_n= (-1)^{m-n}t^{2n-m}e^{(m)}_{m-n} \tag{4}
$$

因此，元素$\theta (t)^2=(-1$0$)$由$(-1)^m$在$V(m)$上运行。如果

0 $-1$

E 是一个奇维简单 $\mathfrak{s}\mathfrak{l}(2, k$) 模，因此 $\theta (t)_E$ 是向量空间 E 的对合自同构。特别是，取 E 为伴随表示：

$$
\theta (t)_EX_+=t^{-2}X_-\theta (t)_EX_-=t^2X_+\theta (t)_EH=-H \tag{5}
$$

因此 $\theta (1)_E=\theta (-1)_E$ 是 $\mathfrak{s}\mathfrak{l}(2, k)$ 的规范对合。

对于任意 $t\in k^*$，将

$$
h(t) =(0tt^-0_1)=\theta (t)\theta (-1)
$$

然后$h(t)u=tu,h(t)v=t^{-1}v$，所以

$$
h(t)e^{(m)}_n=t^{m-2n}e^{(m)}_n \tag{6}
$$

#### 命题 6 {#lie-viii-s1-prop-6 .statement tag=01L4}

令 E 为有限维 $\mathfrak{s}\mathfrak{l}(2, k)$ 模，且为 $t\in k^*$。设$E_p$为权$p$E元素集合。

(i) 从$E_p$到$E_{-p}$，$\theta (t)_E|E_p$是双射。

(ii) $h(t)_E|E_p$ 是位似，$t^p$ 与$E_p$ 的比率。

如果$E = V(n)$，则从公式 (4) 和 (6) 得出命题。一般情况来自 Th。 1.

#### 推论{#lie-viii-s1-n5-cor-1 .statement tag=00YD}

令 $E = E'\oplus E''$ 为 Cor 中定义的 E 的分解。提案 2. $\mathbf{S}\mathbf{L}(2, k)$ 的元素 $(-10)$ 在 $E'$ 上按 +1 运算

0 $-1$

$-1$ $E''$ 前。

这是从适用于 $t=-1$ 的 (ii) 得出的。

### 习题 {#lie-viii-s1-exercises}

基域 $k$ 假定为特征零。

除非另有明确说明，李代数被假定为有限维。

我们用$\mathfrak{s}$李代数$\mathfrak{s}\mathfrak{l}(2, k)$表示。

§ 1](exercises/s1/)参见[习题。
