---
book: lie
book_title: Lie Groups and Lie Algebras
chapter: VIII
chapter_title: SPLIT SEMI-SIMPLE LIE ALGEBRAS
section: 8
section_title: Symmetric invariants
lang: vi
source: lie-vii-ix
book_pages: 141-151, 250-253
pdf_pages: 0149-0159, 0258-0261
extraction: native+ocr
subsections:
    - "no": 1
      title: EXPONENTIAL OF A LINEAR FORM
      page: 141
      pdf_page: 149
    - "no": 2
      title: INJECTION OF $\boldsymbol{k}$[P] INTO S($\mathfrak{h}$)$^*$
      page: 142
      pdf_page: 150
    - "no": 3
      title: INVARIANT POLYNOMIAL FUNCTIONS
      page: 143
      pdf_page: 151
    - "no": 4
      title: PROPERTIES OF Aut0
      page: 148
      pdf_page: 156
    - "no": 5
      title: CENTRE OF THE ENVELOPING ALGEBRA
      page: 148
      pdf_page: 156
statements: 24
exercises: 18
content_sha256: ea084dca96343531fa829ce1d1882d2f790343159c6f7acca817e7e246c05404
translated_from: content/en/lie/VIII/08_s8_symmetric_invariants.md
source_content_sha256: 24cd43812ef1976a490cf9851e6095dc2002480d9c6d6f45be98dfa57b86113e
translation_model: gpt-5-6-mini, gpt-5-6
translation_run: translate-vi-6f37fd3e
glossary_version: 34
glossary_terms_sha256: cf22f4acf83255139be390392d195912712988e285f74513b533549348b040e9
prompt_sha256: 83b0139ff219095b0a7a24ef29a6e4741b2ee7f67a6376a31a9f6aa03aebf5b5
---

## § 8. CÁC BẤT BIẾN ĐỐI XỨNG

Trong đoạn này, ta ký hiệu bởi $(\mathfrak{g},\mathfrak{h})$ một đại số Lie nửa đơn tách, bởi R hệ nghiệm của nó, bởi W nhóm Weyl của nó, và bởi P nhóm các trọng số của nó.

### 1. HÀM MŨ CỦA MỘT DẠNG TUYẾN TÍNH

Cho V là một không gian vectơ hữu hạn chiều, $\mathbf{S}(V)$ là đại số đối xứng của nó. Cấu trúc đại số đối của $\mathbf{S}(V)$ xác định trên $\mathbf{S}(V)^*$ một cấu trúc đại số giao hoán và kết hợp (Đại số, Chương III, §11, tr. 579 đến 582). Không gian vectơ $\mathbf{S}(V)^*$ có thể được đồng nhất một cách chính tắc với $\prod_{m\geq 0}\mathbf{S}^m(V)^*$, và $\mathbf{S}^m(V)^*$ có thể

được đồng nhất một cách chính tắc với không gian các dạng đối xứng $m$-tuyến tính trên V. Đơn ánh chính tắc của $V^*=\mathbf{S}^1(V)^*$ vào $\mathbf{S}(V)^*$ xác định một đơn cấu từ đại số $\mathbf{S}(V^*)$ vào đại số $\mathbf{S}(V)^*$, có ảnh là $\mathbf{S}(V)^{*gr}=\sum_{m\geq 0}\mathbf{S}^m(V)^*($Đại số, Chương III, §11, no. 5, Mệnh đề 8). Ta đồng nhất

các đại số $\mathbf{S}(V^*)$ và $\mathbf{S}(V)^{*gr}$ bằng đồng cấu này; ta cũng đồng nhất $\mathbf{S}(V^*)$ với đại số các hàm đa thức trên V (Chương VII, Phụ lục I, no. 1).

Các phần tử $(u_m)\in \prod_{m\geq 0}\mathbf{S}^m(V)^*$ sao cho $u_0= 0$ tạo thành một iđêan J của

$\mathbf{S}(V)^*$; ta trang bị cho $\mathbf{S}(V)^*$ tôpô J-adic (Đại số giao hoán, Chương III, §2, no. 5), trong đó $\mathbf{S}(V)^*$ là đầy đủ và $\mathbf{S}(V^*)$ là trù mật trong $\mathbf{S}(V)^*$. Nếu $(e^*_i)_{1\leq i\leq n}$ là một cơ sở của $V^*$, và nếu $T_1, . . . ,T_n$ là các bất định, đồng cấu từ $k[T_1, . . . ,T_n]$ vào $\mathbf{S}(V^*)$ nhận $T_i$ thành $e^*_i(1\leq i\leq n)$ là một đẳng cấu các đại số, và mở rộng thành một đẳng cấu liên tục từ đại số $k[[T_1, . . . ,T_n]]$ vào đại số $\mathbf{S}(V)^*$.

Với mọi $\lambda \in V^*$, họ $\lambda^n/n$! là khả tổng trong $\mathbf{S}(V)^*$. Tổng của nó được gọi là hàm mũ của $\lambda$ và được ký hiệu bởi exp($\lambda$ ) (phù hợp với Chương II, §6, no. 1). Cho $x_1, . . . , x_n\in V$; ta có

$\langle$exp $\lambda , x_1. . . x_n\rangle =n1$!$\langle \lambda^n, x_1. . . x_n\rangle =\langle \lambda , x_1\rangle . . .\langle \lambda , x_n\rangle$

theo Đại số, Chương III, §11, no. 5, công thức (29). Suy ra ngay lập tức rằng exp($\lambda$ ) là đồng cấu duy nhất từ đại số $\mathbf{S}(V)$ vào $k$ mở rộng $\lambda$.

Ta có exp($\lambda +\mu$) $=$ exp($\lambda$ ) exp($\mu$) với mọi $\lambda , \mu\in V^*$ (Chương II, §6, no. 1, Nhận xét). Do đó, ánh xạ exp$: V^*\rightarrow \mathbf{S}(V)^*$ là một đồng cấu từ nhóm cộng $V^*$ vào nhóm nhân các phần tử khả nghịch của $\mathbf{S}(V)^*$. Họ (exp $\lambda$ )$_{\lambda\in V^*}$ là một họ tự do trong không gian vectơ $\mathbf{S}(V)^*($Đại số, Chương V, §7, no. 3, Định lý 1).

#### Bổ đề 1 {#lie-viii-s8-lem-1 .statement tag=0154}

Cho $\Pi$ là một nhóm con của $V^*$ sinh ra không gian vectơ $V^*$, và $m$ là một số nguyên $\geq 0$. Khi đó pr$_m$(exp $\Pi$ ) sinh ra không gian vectơ $\mathbf{S}^m(V^*)$.

Theo Đại số, Ch. I, §8, no. 2, Mệnh đề 2, mọi tích của $m$ phần tử của $V^*$ là một tổ hợp $k$-tuyến tính của các phần tử có dạng $x^m$ với $x\in \Pi$. Nhưng $x^m=m$! pr$_m$(exp $x$). Q.E.D.

Bằng phép chuyển cấu trúc, mọi tự đẳng cấu của V xác định các tự đẳng cấu của các đại số $\mathbf{S}(V)$ và $\mathbf{S}(V)^*$; điều này cho các biểu diễn tuyến tính của $\mathbf{G}\mathbf{L}(V)$ trên $\mathbf{S}(V)$ và $\mathbf{S}(V)^*$.

### 2. ĐƠN ÁNH CỦA $\boldsymbol{k}$[P] VÀO S($\mathfrak{h}$)$^*$

Ánh xạ $p \rightarrow$ exp $p$ từ P vào $\mathbf{S}(\mathfrak{h})^*$ là một đồng cấu từ nhóm cộng P vào $\mathbf{S}(\mathfrak{h})^*$ được trang bị cấu trúc nhân của nó (no. 1). Do đó, tồn tại một đồng cấu duy nhất $\psi$ từ đại số $k[P]$ của monoid P vào đại số $\mathbf{S}(\mathfrak{h})^*$ sao cho

$\psi (e^{\lambda}) =$ exp($\lambda$ )$(\lambda \in P)$

(theo các ký hiệu của §7, no. 7). Theo số $1,\psi$ là đơn ánh. Bằng phép chuyển cấu trúc, $\psi (w(e^{\lambda})) =w(\psi (e^{\lambda}))$ với mọi $\lambda \in P$ và mọi $w\in W$. Do đó, nếu $k[P]^W$ (tương ứng $\mathbf{S}(\mathfrak{h})^{*W}$) ký hiệu tập hợp các phần tử của $k[P]$ (tương ứng $\mathbf{S}(\mathfrak{h})^*$) bất biến dưới W, ta có $\psi (k[P]^W)\subset \mathbf{S}(\mathfrak{h})^{*W}$.

#### Mệnh đề 1 {#lie-viii-s8-prop-1 .statement tag=0155}

Cho $S^m(\mathfrak{h}^*)^W$ là tập hợp các phần tử của $S^m(\mathfrak{h}^*)$ bất biến dưới W. Khi đó pr$_m(\psi (k[P]^W)) =\mathbf{S}^m(\mathfrak{h}^*)^W$.

Hiển nhiên từ điều đã nêu trước đó rằng pr$_m(\psi (k[P]^W))\subset \mathbf{S}^m(\mathfrak{h}^*)^W$. Mọi phần tử của $\mathbf{S}^m(\mathfrak{h}^*)$ là một tổ hợp $k$-tuyến tính của các phần tử có dạng

pr$_m$(exp $\lambda$ ) $=$ (pr$_m\circ \psi$ )$(e^{\lambda})$

trong đó $\lambda \in P$ (Bổ đề 1). Do đó mọi phần tử của $\mathbf{S}^m(\mathfrak{h}^*)^W$ là một tổ hợp tuyến tính của các phần tử có dạng

$\sum_{w\in W}w$((pr$_m\circ \psi$ )$(e^{\lambda})$) $=$ (pr$_m\circ \psi$ )$(\sum_{w\in W}w(e^{\lambda}))$,

mỗi phần tử trong đó đều thuộc pr$_m(\psi (k[P]^W))$.

#### Mệnh đề 2 {#lie-viii-s8-prop-2 .statement tag=0156}

Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều. Cho $U(\mathfrak{h}) =\mathbf{S}(\mathfrak{h})$ là đại số bao của $\mathfrak{h}$. Nếu $u\in U(\mathfrak{h})$, thì

Tr($u_E$) $=\langle \psi$(ch $E$)$, u\rangle$.

Chỉ cần xét trường hợp trong đó $u=h_1. . . h_m$ với $h_1, . . . , h_m\in \mathfrak{h}$. Với mọi $\lambda \in P$, đặt $d_{\lambda}=$ dim $E^{\lambda}$. Khi đó ch $E =\sum_{\lambda}d_{\lambda}e^{\lambda}$, do đó $\psi$(ch $E$) $=\sum_{\lambda}d_{\lambda}$ exp($\lambda$ ) và vì thế

$$
\langle \psi(\mathrm{ch}\,E),u\rangle
 = \sum_{\lambda} d_\lambda\langle\exp\lambda,h_1\ldots h_m\rangle
$$
$$
= \sum_{\lambda} d_\lambda\lambda(h_1)\ldots\lambda(h_m)\qquad\text{(no. 1)}
$$
$$
= \mathrm{Tr}\,u_E.
$$

#### Hệ quả 1 {#lie-viii-s8-prop-2-cor-1 .statement tag=01J7}

— Cho $\mathrm{U}(\mathfrak g)$ là đại số bao của $\mathfrak g$. Cho đồng cấu
$$
\zeta:\mathrm{U}(\mathfrak g)^*\longrightarrow\mathrm{U}(\mathfrak h)^*=\mathrm{S}(\mathfrak h)^*
$$
là chuyển vị của đơn ánh chính tắc
$$
\mathrm{U}(\mathfrak h)\longrightarrow\mathrm{U}(\mathfrak g).
$$
Biểu đồ sau giao hoán
$$
\begin{array}{ccccc}
\mathscr{R}(\mathfrak g)&\xrightarrow{\mathrm{ch}}&\mathbf{Z}[P]\\
\Big\downarrow{\scriptstyle\mathrm{Tr}}&&\Big\downarrow{\scriptstyle\psi}\\
\mathrm{U}(\mathfrak g)^*&\xrightarrow{\zeta}&\mathrm{S}(\mathfrak h)^*
\end{array}
$$

Đây chỉ đơn giản là một cách phát biểu lại Mệnh đề 2.

#### Hệ quả 2 {#lie-viii-s8-prop-2-cor-2 .statement tag=01J8}

— Cho $m$ là một số nguyên $\geqslant 0$. Mọi phần tử của $\mathrm{S}^m(\mathfrak h^*)^W$ là một tổ hợp tuyến tính của các hàm đa thức trên $\mathfrak h$ có dạng $x\mapsto\mathrm{Tr}(\rho(x)^m)$, trong đó $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak g$.

Theo Mệnh đề 1, $\mathrm{S}^m(\mathfrak h^*)^W=(\mathrm{pr}_m\circ\psi)(k[P]^W)$. Bây giờ $\mathbf{Z}[P]^W=\mathrm{ch}\,\mathscr{R}(\mathfrak g)$ (§7, no. 7, Định lý 2 (ii)). Do đó, theo Chương VI, §3, no. 4, Bổ đề 3, $\psi(k[P]^W)$ là không gian con vectơ trên $k$ của $\mathrm{S}(\mathfrak h)^*$ được sinh bởi $\psi(\mathrm{ch}\,\mathscr{R}(\mathfrak g))=\zeta(\mathrm{Tr}\,\mathscr{R}(\mathfrak g))$. Do đó, $\mathrm{S}^m(\mathfrak h^*)^W$ là không gian con vectơ của $\mathrm{S}^m(\mathfrak h^*)$ được sinh bởi $(\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\mathscr{R}(\mathfrak g))$. Nhưng, nếu $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak g$,

$$
((\mathrm{pr}_m\circ\zeta\circ\mathrm{Tr})(\rho))(x)
=\left\langle(\zeta\circ\mathrm{Tr})(\rho),\frac{x^m}{m!}\right\rangle
=\frac{1}{m!}\mathrm{Tr}(\rho(x)^m)
$$

với mọi $x\in\mathfrak h$.

### 3. CÁC HÀM ĐA THỨC BẤT BIẾN

Cho $\mathfrak a$ là một đại số Lie hữu hạn chiều. Theo các quy ước của no. 1, ta đồng nhất đại số $\mathrm{S}(\mathfrak a^*)$, đại số $\mathrm{S}(\mathfrak a)^{*gr}$, và đại số các hàm đa thức trên $\mathfrak a$. Với mọi $a\in\mathfrak a$, gọi $\theta(a)$ là đạo hàm của $\mathrm{S}(\mathfrak a)$ sao cho $\theta(a)x=[a,x]$ với mọi $x\in\mathfrak a$. Ta biết (Chương I, §3, no. 2) rằng $\theta$ là một biểu diễn của $\mathfrak a$ trên $\mathrm{S}(\mathfrak a)$. Gọi $\theta^*(\mathfrak a)$ là hạn chế của ${}^t\theta(a)$ lên $\mathrm{S}(\mathfrak a^*)$. Khi đó $\theta^*$ là một biểu diễn của $\mathfrak a$. Nếu $f\in\mathrm{S}^n(\mathfrak a^*)$, thì $\theta^*(a)f\in\mathrm{S}^n(\mathfrak a^*)$ và, với $x_1,\ldots,x_n\in\mathfrak a$,

$$
(\theta^*(a)f)(x_1,\ldots,x_n)
=-\sum_{1\leqslant i\leqslant n}
f(x_1,\ldots,x_{i-1},[a,x_i],x_{i+1},\ldots,x_n).
\tag{1}
$$

Ta dễ dàng suy ra từ (1) rằng $\theta^*(a)$ là một đạo hàm của $\mathbf{S}(\mathfrak{a}^*)$. Một phần tử của $\mathbf{S}(\mathfrak{a})$ (tương ứng $\mathbf{S}(\mathfrak{a}^*)$) bất biến đối với biểu diễn $\theta$ (tương ứng $\theta^*$) của $\mathfrak{a}$ được gọi là một phần tử bất biến của $\mathbf{S}(\mathfrak{a})$ (tương ứng $\mathbf{S}(\mathfrak{a}^*)$).

#### Bổ đề 2 {#lie-viii-s8-lem-2 .statement tag=0157}

Cho $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{a}$, và $m$ là một số nguyên $\geq 0$. Hàm $x \rightarrow$ Tr($\rho (x)^m$) trên $\mathfrak{a}$ là một hàm đa thức bất biến.

Đặt $g(x_1, . . . , x_m) =$ Tr($\rho (x_1). . . \rho (x_m)$) với $x_1, . . . , x_m\in \mathfrak{a}$. Nếu $x\in \mathfrak{a}$, ta có

$$
-(\theta^*(x)g)(x_1, . . . , x_m)
$$

$=\sum_{1\leq i\leq m}$ Tr($\rho (x_1). . . \rho (x_{i-1})[\rho (x), \rho (x_i)]\rho (x_{i+1}). . . \rho (x_m)$)

= Tr($\rho (x)\rho (x_1). . . \rho (x_m)$)$-$ Tr($\rho (x_1). . . \rho (x_m)\rho (x)$) $= 0$,

do đó $\theta^*(x)g= 0$. Gọi $h$ là dạng đa tuyến tính đối xứng được xác định bởi

$h(x_1, . . . , x_m) =m1$! $\sum g(x_{\sigma(1)}, . . . , x_{\sigma(m)})$.

$\sigma \in \mathfrak{S}_m$

Với mọi $x\in \mathfrak{a}$, ta có $\theta^*(x)h= 0$ và Tr($\rho (x)^m$) $=h(x, . . . , x)$, do đó bổ đề được chứng minh.

#### Bổ đề 3 {#lie-viii-s8-lem-3 .statement tag=0158}

Cho E là một $\mathfrak{g}$-môđun hữu hạn chiều, và $x\in E$. Khi đó $x$ là một phần tử bất biến của $\mathfrak{g}$-môđun E khi và chỉ khi (exp $a_E$)$.x=x$ với mọi phần tử lũy linh $a$ của $\mathfrak{g}$.

Điều kiện này rõ ràng là cần thiết. Giả sử bây giờ nó được thỏa mãn. Cho $a$ là một phần tử lũy linh của $\mathfrak{g}$. Tồn tại một số nguyên $n$ sao cho $a^n_E= 0$. Với mọi $t\in k$, ta có

$0 = \exp(ta_E).x - x = ta_Ex + \frac{1}{2!}t^2a^2_Ex + \cdots + \frac{1}{(n-1)!}t^{n-1}a^{n-1}_Ex,$

suy ra $a_Ex= 0$. Nhưng đại số Lie $\mathfrak{g}$ được sinh bởi các phần tử lũy linh của nó (§4, no. 1, Mệnh đề 1). Do đó $x$ là một phần tử bất biến của $\mathfrak{g}$-môđun E. Q.E.D.

Với mọi $\xi \in \mathbf{G}\mathbf{L}(\mathfrak{g})$, gọi $\mathbf{S}(\xi )$ là tự đẳng cấu của $\mathbf{S}(\mathfrak{g})$ mở rộng $\xi$, và $\mathbf{S}^*(\xi )$ là hạn chế lên $\mathbf{S}(\mathfrak{g}^*)$ của tự đẳng cấu đối ngẫu của $\mathbf{S}(\xi )$. Khi đó $\mathbf{S}$ và $\mathbf{S}^*$ là các biểu diễn của $\mathbf{G}\mathbf{L}(\mathfrak{g})$. Nếu $a$ là một phần tử lũy linh của $\mathfrak{g},\theta (a)$ là lũy linh địa phương trên $\mathbf{S}(\mathfrak{g})$ và $\mathbf{S}$(exp ad $a$) $=$ exp$\theta (a)$, do đó

$\mathbf{S}^*$(exp ad $a$) $=$ exp$\theta^*(a)$. (2)

#### Mệnh đề 3 {#lie-viii-s8-prop-3 .statement tag=0159}

Cho $f$ là một hàm đa thức trên $\mathfrak{g}$. Các điều kiện sau là tương đương:

(i) $f\circ s=f$ for all $s\in$ Aut$_e(\mathfrak{g})$;

(ii) $f\circ s=f$ for all $s\in$ Aut$_0(\mathfrak{g})$;

(iii) $f$ is invariant.

Sự tương đương của (i) và (iii) suy ra từ công thức (2) và Bổ đề 3. Từ đó suy ra rằng (iii) kéo theo (ii) bằng mở rộng trường cơ sở. Kéo theo (ii) $=\Rightarrow$ (i) là rõ ràng.

Cần chú ý kỹ rằng, nếu $f$ thỏa mãn các điều kiện của Mệnh đề $3,f$ nói chung không bất biến dưới Aut($\mathfrak{g}$) (Bài tập 1 và 2).

#### Định lý 1 {#lie-viii-s8-thm-1 .statement tag=015A}

Cho $I(\mathfrak{g}^*)$ là đại số của các hàm đa thức bất biến trên $\mathfrak{g}$. Gọi $i:\mathbf{S}(\mathfrak{g}^*)\rightarrow \mathbf{S}(\mathfrak{h}^*)$ là đồng cấu hạn chế.

(i) Ánh xạ $i|I(\mathfrak{g}^*)$ là một đẳng cấu từ đại số $I(\mathfrak{g}^*)$ đến đại số $\mathbf{S}(\mathfrak{h}^*)^W$.

(ii) Với mọi số nguyên $n\geq 0$, gọi $I^n(\mathfrak{g}^*)$ là tập hợp các phần tử thuần nhất của $I(\mathfrak{g}^*)$ có bậc $n$. Khi đó $I^n(\mathfrak{g}^*)$ là tập hợp các tổ hợp tuyến tính của các hàm trên $\mathfrak{g}$ có dạng $x \rightarrow$ Tr($\rho (x)^n$), trong đó $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{g}$.

(iii) Gọi $l=$ rk($\mathfrak{g}$). Tồn tại $l$ phần tử thuần nhất độc lập đại số của $I(\mathfrak{g}^*)$ sinh đại số $I(\mathfrak{g}^*)$.

a) Cho $f\in I(\mathfrak{g}^*)$ và $w\in W$. Tồn tại $s\in$ Aut$_e(\mathfrak{g},\mathfrak{h})$ sao cho $s|\mathfrak{h}=w($§2, no. 2, Cor. of Th. 2). Vì $f$ là bất biến dưới tác động của $s$ (Mệnh đề $3$)$,i(f)$ là bất biến dưới tác động của $w$. Do đó $i(I(\mathfrak{g}^*))\subset \mathbf{S}(\mathfrak{h}^*)^W$.

b) Ta chứng minh rằng, nếu $f\in I(\mathfrak{g}^*)$ sao cho $i(f) = 0$, thì $f= 0$. Nếu cần thiết, mở rộng trường cơ sở, ta có thể giả sử rằng $k$ là đóng đại số. Theo Mệnh đề $3,f$ triệt tiêu trên $s(\mathfrak{h})$ với mọi $s\in$ Aut$_e(\mathfrak{g})$. Do đó $f$ triệt tiêu trên mọi đại số con Cartan của $\mathfrak{g}$ (Chap. VII, §3, no. 2, Th. 1), và đặc biệt trên tập hợp các phần tử chính quy của $\mathfrak{g}$. Nhưng tập hợp này trù mật trong $\mathfrak{g}$ đối với tôpô Zariski (Chap. VII, §2, no. 2).

c) Cho $n$ là một số nguyên $\geq 0$. Gọi $L^n$ là tập hợp các tổ hợp tuyến tính của các hàm có dạng $x \rightarrow$ Tr($\rho (x)^n$) trên $\mathfrak{g}$, trong đó $\rho$ là một biểu diễn tuyến tính hữu hạn chiều của $\mathfrak{g}$. Theo Bổ đề $2, L^n\subset I^n(\mathfrak{g}^*)$. Do đó

$$
i(L^n)\subset i(I^n(\mathfrak{g}^*))\subset \mathbf{S}^n(\mathfrak{h}^*)^W
$$

Theo Hệ quả 2 của Mệnh đề $2,\mathbf{S}^n(\mathfrak{h}^*)^W\subset i(L^n)$. Suy ra $i(I^n(\mathfrak{g}^*)) =\mathbf{S}^n(\mathfrak{h}^*)^W$, điều này chứng minh (i), và $i(L^n) =i(I^n(\mathfrak{g}^*))$ nên $L^n= I^n(\mathfrak{g}^*)$ theo b). Vậy (ii) được chứng minh.

d) Mệnh đề (iii) suy ra từ (i) và Chap. V, §5, no. 3, Th. 3.

#### Hệ quả 1 {#lie-viii-s8-thm-1-cor-1 .statement tag=015B}

Giả sử rằng $\mathfrak{g}$ là đơn. Cho $m_1, . . . , m_l$ là các số mũ của nhóm Weyl của $\mathfrak{g}$. Có các phần tử $P_1, . . . ,P_l$ của $I(\mathfrak{g}^*)$, thuần nhất với các bậc

$$
m_1+ 1, . . . , m_l+ 1
$$

độc lập đại số và sinh đại số $I(\mathfrak{g}^*)$.

Điều này suy ra từ Định lý 2 (i) và Chương V, §6, no. 2, Mệnh đề 3.

#### Hệ quả 2 {#lie-viii-s8-thm-1-cor-2 .statement tag=015C}

Cho B là một cơ sở của R, $R_+$ (tương ứng $R_-$) là tập hợp các nghiệm dương (tương ứng âm) của $(\mathfrak{g},\mathfrak{h})$ đối với B$,\mathfrak{n}_+=\sum_{\alpha\in R_+}\mathfrak{g}^{\alpha},\mathfrak{n}_-=\sum_{\alpha\in R_-}\mathfrak{g}^{\alpha}$, $\mathbf{S}(\mathfrak{h})$ là đại số đối xứng của $\mathfrak{h}$, và J là iđêan của $\mathbf{S}(\mathfrak{g})$ sinh bởi $\mathfrak{n}_+\cup \mathfrak{n}_-$.

(i) $\mathbf{S}(\mathfrak{g}) =\mathbf{S}(\mathfrak{h})\oplus J$.

(ii) Cho $j$ là đồng cấu từ đại số $\mathbf{S}(\mathfrak{g})$ vào đại số $\mathbf{S}(\mathfrak{h})$ được xác định bởi phân tích trước đó của $\mathbf{S}(\mathfrak{g})$. Cho $I(\mathfrak{g})$ là tập hợp các phần tử bất biến của $\mathbf{S}(\mathfrak{g})$. Cho $\mathbf{S}(\mathfrak{h})^W$ là tập hợp các phần tử của $\mathbf{S}(\mathfrak{h})$ bất biến đối với phép toán của W. Khi đó $j|I(\mathfrak{g})$ là một đẳng cấu từ $I(\mathfrak{g})$ đến $\mathbf{S}(\mathfrak{h})^W$.

Mệnh đề (i) là rõ ràng. Dạng Killing xác định một đẳng cấu từ không gian vectơ $\mathfrak{g}^*$ đến không gian vectơ $\mathfrak{g}$, nó mở rộng thành một đẳng cấu $\xi$ từ $\mathfrak{g}$-môđun $\mathbf{S}(\mathfrak{g}^*)$ đến $\mathfrak{g}$-môđun $\mathbf{S}(\mathfrak{g})$. Ta có $\xi (I(\mathfrak{g}^*)) = I(\mathfrak{g})$. Phần bù trực giao của $\mathfrak{h}$ đối với dạng Killing là $\mathfrak{n}_++\mathfrak{n}_-($§2, no. 2, Mệnh đề 1). Nếu ta đồng nhất $\mathfrak{h}^*$ với phần bù trực giao của $\mathfrak{n}_++\mathfrak{n}_-$ trong $\mathfrak{g}^*$, thì $\xi (\mathfrak{h}^*) =\mathfrak{h}$, do đó $\xi (\mathbf{S}(\mathfrak{h}^*)) =\mathbf{S}(\mathfrak{h})$ và $\xi (\mathbf{S}(\mathfrak{h}^*)^W) =\mathbf{S}(\mathfrak{h})^W$. Cuối cùng, $\xi^{-1}(J)$ là tập hợp các hàm đa thức trên $\mathfrak{g}$ triệt tiêu trên $\mathfrak{h}$. Điều này chứng minh rằng $\xi$ biến đồng cấu $i$ của Định lý 1 thành đồng cấu $j$ của Hệ quả 2. Do đó mệnh đề (ii) suy ra từ Định lý 1 (i).

#### Mệnh đề 4 {#lie-viii-s8-prop-4 .statement tag=015D}

Cho $\mathfrak{a}$ là một đại số Lie nửa đơn, $l$ là hạng của nó. Cho I (tương ứng $I'$) là tập hợp các phần tử của $\mathbf{S}(\mathfrak{a}^*)$ (tương ứng $\mathbf{S}(\mathfrak{a})$) bất biến dưới biểu diễn cảm sinh bởi biểu diễn phụ hợp của $\mathfrak{a}$. Cho Z là tâm của đại số bao phủ của $\mathfrak{a}$.

(i) I và $I'$ là các đại số đa thức phân bậc (Chương V, §5, no. 1) có bậc siêu việt $l$.

(ii) Z đẳng cấu với đại số các đa thức theo $l$ bất định trên $k$.

Lọc chính tắc của đại số bao quanh của $\mathfrak{a}$ cảm sinh một lọc của Z. Theo Chương I, §2, no. 7, Định lý 1 và p. 25, gr Z đẳng cấu với $I'$. Theo Đại số giao hoán, Chương III, §2, no. 9, Mệnh đề 10, suy ra rằng (i) $=\Rightarrow$ (ii).

Mặt khác, Định lý 1 và Hệ quả 2 của nó chỉ ra rằng (i) đúng khi $\mathfrak{a}$ là tách. Trường hợp tổng quát quy về trường hợp đó theo bổ đề sau:

#### Bổ đề 4 {#lie-viii-s8-lem-4 .statement tag=01JY}

$^2$ Cho $A =\bigoplus_{n\geq 0}A^n$ là một đại số $k$ phân bậc, $k'$ là một mở rộng của $k$, và $A'= A\otimes_kk'$. Giả sử rằng $A'$ là một đại số đa thức phân bậc trên $k'$. Khi đó A là một đại số đa thức phân bậc trên $k$.

Ta có ${A'}^0=k'$, do đó $A^0=k$. Đặt $A_+=\bigoplus_{n\geq 1}A^n$ và $P = A_+/A^2_+$. Khi đó P là một không gian vectơ phân bậc, và có một ánh xạ tuyến tính phân bậc $f: P\rightarrow A_+$ có

$^2$ Trong các Bổ đề 4, 5 và $6,k$ có thể là một trường (giao hoán) bất kỳ. bậc không sao cho hợp thành với phép chiếu chính tắc $A_+\rightarrow P$ là đồng nhất trên P. Cho $\mathbf{S}(P)$ cấu trúc phân bậc cảm sinh bởi cấu trúc của P (Đại số, Chương III, p. 506). Đồng cấu của các đại số $k$ $g:\mathbf{S}(P)\rightarrow A$ mở rộng $f$ (Đại số, Chương III, p. 497) là một đồng cấu phân bậc bậc 0; một phép quy nạp ngay lập tức theo bậc chỉ ra rằng $g$ là toàn ánh.

#### Bổ đề 5 {#lie-viii-s8-lem-5 .statement tag=015E}

A là một đại số đa thức phân bậc khi và chỉ khi P hữu hạn chiều và $g$ là song ánh.

Nếu P hữu hạn chiều, $\mathbf{S}(P)$ rõ ràng là một đại số đa thức phân bậc, và A cũng vậy nếu $g$ là song ánh. Ngược lại, giả sử rằng A được sinh bởi các phần tử thuần nhất độc lập đại số $x_1, . . . , x_m$ có các bậc $d_1, . . . , d_m$. Gọi $\overline{x}_i$ là ảnh của $x_i$ trong P. Hiển nhiên rằng các $\overline{x}_i$ tạo thành một cơ sở của P; vì $\overline{x}_i$ có bậc $d_i$, suy ra rằng $\mathbf{S}(P)$ và A đẳng cấu; đặc biệt, dim $\mathbf{S}(P)^n=$ dim $A^n$ với mọi $n$. Vì $g$ là toàn ánh, nó nhất thiết là song ánh.

Bổ đề 4 bây giờ là ngay lập tức. Thật vậy, Bổ đề 5, áp dụng cho đại số $k'$ $A'$, chỉ ra rằng $g\otimes 1 :\mathbf{S}(P)\otimes k'\rightarrow A\otimes k'$ là song ánh, và do đó $g$ cũng vậy.

#### Mệnh đề 5 {#lie-viii-s8-prop-5 .statement tag=015F}

Ta giữ các ký hiệu của Mệnh đề 4, và ký hiệu $\mathfrak{p}$ là iđêan của $\mathbf{S}(\mathfrak{a}^*)$ sinh bởi các phần tử thuần nhất của I có bậc $\geq 1$. Cho $x\in \mathfrak{a}$. Khi đó $x$ là lũy linh khi và chỉ khi $f(x) = 0$ với mọi $x\in \mathfrak{p}.^3$

Mở rộng trường cơ sở nếu cần, ta có thể giả sử rằng $\mathfrak{a}=\mathfrak{g}$ là tách được. Giả sử rằng $x$ là lũy linh. Với mọi biểu diễn tuyến tính hữu hạn chiều $\rho$ của $\mathfrak{g}$, và mọi số nguyên $n\geq 1$, ta có Tr($\rho (x)^n$) $= 0$, do đó $f(x) = 0$ với mọi $f\in I(\mathfrak{g}^*)$ thuần nhất có bậc $\geq 1$ (Th. 1 (ii)), và vì vậy $f(x) = 0$ với mọi $f\in \mathfrak{p}$. Ngược lại, nếu $f(x) = 0$ với mọi $f\in \mathfrak{p}$, thì Tr((ad $x$)$^n$) $= 0$ với mọi $n\geq 1$ (Th. 1 (ii)), do đó $x$ là lũy linh.

#### Nhận xét 1 {#lie-viii-s8-n3-rem-1 .statement tag=01L5}

$^*$Cho $P_1, . . . ,P_l$ là các phần tử thuần nhất độc lập đại số của I sinh ra đại số I. Khi đó $(P_1, . . . ,P_l)$ là một dãy $\mathbf{S}(\mathfrak{a}^*)$-chính quy (Chương V, §5, no. 5). Thật vậy, mở rộng trường cơ sở nếu cần, ta có thể giả sử rằng $\mathfrak{a}=\mathfrak{g}$ là tách được. Bây giờ đặt N = dim $\mathfrak{g}$, và cho

$$
(Q_1, . . . ,Q_{N-l})
$$

là một cơ sở của phần bù trực giao của $\mathfrak{h}$ trong $\mathfrak{g}^*$. Gọi $\mathfrak{m}$ là iđêan của $\mathbf{S}(\mathfrak{g}^*)$ sinh bởi $P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l}$. Khi đó $\mathbf{S}(\mathfrak{g}^*)\mathfrak{m}$ đẳng cấu với $\mathbf{S}(\mathfrak{h}^*)/J$, trong đó J là iđêan của $\mathbf{S}(\mathfrak{h}^*)$ sinh bởi $i(P_1), . . . , i(P_l)$. Theo Th. 1 và Chương V, §5, no. 2, Th. $2,\mathbf{S}(\mathfrak{h}^*)/J$ là một không gian vectơ hữu hạn chiều, và do đó $\mathbf{S}(\mathfrak{g}^*)/\mathfrak{m}$ cũng vậy. Theo một kết quả của Đại số giao hoán, suy ra rằng $(P_1, . . . ,P_l,Q_1, . . . ,Q_{N-l})$ là một dãy $\mathbf{S}(\mathfrak{g}^*$)-chính quy, và a fortiori $(P_1, . . . ,P_l)$ cũng vậy.

$^3$ Có thể chỉ ra (B. KOSTANT, Lie group representations on polynomial rings,

Amer. J. Math., Vol. LXXXV (1963), pp. 327-404, Th. 10 and 15) rằng $\mathfrak{p}$ là một

iđêan nguyên tố của $\mathbf{S}(\mathfrak{a}^*)$ và rằng $\mathbf{S}(\mathfrak{a}^*)/\mathfrak{p}$ là đóng nguyên.

#### Nhận xét 2 {#lie-viii-s8-n3-rem-2 .statement tag=01L6}

Đại số $\mathbf{S}(\mathfrak{a}^*)$ là một môđun tự do phân bậc trên I. Thật vậy, điều này suy ra từ Mệnh đề 4, Nhận xét 1, và Chương V, §5, no. 5, Bổ đề $5._*$

### 4. CÁC TÍNH CHẤT CỦA Aut0

#### Bổ đề 6 {#lie-viii-s8-lem-6 .statement tag=015G}

Cho V là một không gian vectơ hữu hạn chiều, G là một nhóm hữu hạn các tự đẳng cấu của V, và $v$ và $v'$ là các phần tử của V sao cho $v'\notin Gv$. Tồn tại một hàm đa thức G-bất biến $f$ trên V sao cho $f(v')\not=f(v)$.

Thật vậy, với mỗi $s\in G$ tồn tại một hàm đa thức $g_s$ trên V bằng 1 tại $v$ và bằng 0 tại $sv'$. Khi đó hàm $g= 1-\prod_{s\in G}g_s$ bằng 0 tại

$v$ và bằng 1 trên $Gv'$. Hàm đa thức $f=\prod_{t\in g}t.g$ là bất biến G, bằng 0 tại $v$ và bằng 1 tại $v'$.

#### Mệnh đề 6 {#lie-viii-s8-prop-6 .statement tag=015H}

Cho $\mathfrak{a}$ là một đại số Lie nửa đơn và $s\in$ Aut($\mathfrak{a}$). Các điều kiện sau là tương đương:

(i) $s\in$ Aut$_0(\mathfrak{a})$;

(ii) với mọi hàm đa thức bất biến $f$ trên $\mathfrak{a}$, ta có $f\circ s=f$.

Bằng cách mở rộng vô hướng nếu cần, ta có thể giả sử rằng $k$ là đóng đại số. Kéo theo (i) $=\Rightarrow$ (ii) suy ra từ Mệnh đề 3. Ta giả sử rằng điều kiện (ii) được thỏa mãn và chứng minh (i). Theo Mệnh đề 3, và §5, no. 3, Hệ quả 1 của Mệnh đề 5, ta có thể giả sử rằng $s\in$ Aut($\mathfrak{g},\mathfrak{h}$) và rằng $s$ giữ ổn định một buồng Weyl C. Cho $x\in C\cap \mathfrak{h}_{\mathbf{Q}}$. Ta có $sx\in C$. Nếu $g$ là một hàm đa thức W-bất biến trên $\mathfrak{h}$, ta có $g(x) =g(sx)$ (Định lý 1 (i)). Theo Bổ đề 6, suy ra rằng $sx\in Wx$. Vì $sx\in C$, ta có $x=sx$ (Chap. V, §3, no. 3, Định lý 2). Khi đó $s|\mathfrak{h}=$ Id$_{\mathfrak{h}}$, và $s\in$ Aut$_0(\mathfrak{g},\mathfrak{h})$ (§5, no. 2, Mệnh đề 4).

#### Hệ quả {#lie-viii-s8-n4-cor-1 .statement tag=015I}

Nhóm Aut$_0(\mathfrak{a})$ là mở và đóng trong Aut($\mathfrak{a}$) đối với tôpô Zariski.

Mệnh đề 6 chỉ ra rằng Aut$_0(\mathfrak{a})$ là đóng. Gọi $\overline{k}$ là một bao đóng đại số của $k$. Nhóm Aut($\mathfrak{a}\otimes \overline{k}$)$/$Aut$_0(\mathfrak{a}\otimes \overline{k})$ là hữu hạn (§5, no. 3, Hệ quả 1 của Mệnh đề 5); a fortiori, nhóm Aut($\mathfrak{a}$)$/$Aut$_0(\mathfrak{a})$ là hữu hạn. Vì các lớp kề của Aut($\mathfrak{a}$) trong Aut($\mathfrak{a}$) là đóng, suy ra rằng Aut$_0(\mathfrak{a})$ là mở trong Aut($\mathfrak{a}$).

### 5. TÂM CỦA ĐẠI SỐ BAO

Trong số này, ta chọn một cơ sở B của R. Cho $R_+$ là tập hợp các nghiệm dương đối với B. Cho $\rho =\frac{1}{2}\sum_{\alpha\in R_+}\alpha$, và $\delta$ là tự đẳng cấu của đại số $\mathbf{S}(\mathfrak{h})$ biến mọi $x\in \mathfrak{h}$ thành $x-\rho (x)$, và do đó hàm đa thức $p$ trên $\mathfrak{h}^*$ thành hàm $\lambda  \rightarrow p(\lambda -\rho )$.

#### Định lý 2 {#lie-viii-s8-thm-2 .statement tag=015J}

Cho $U$ là đại số bao quanh của $\mathfrak{g}$, Z là tâm của nó, $V\subset U$ là đại số bao quanh của $\mathfrak{h}($đồng nhất với $\mathbf{S}(\mathfrak{h}))$, $U^0$ là hoán tập của V trong U, $\varphi$ là *đồng cấu Harish-Chandra* (§6, no. 4) từ $U^0$ đến $V$ tương đối với $B$.

Cho $S(\mathfrak h)^W$ là tập hợp các phần tử của $S(\mathfrak h)$ bất biến đối với tác động của $W$. Khi đó $(\delta\circ\varphi)|_Z$ là một đẳng cấu từ $Z$ đến $S(\mathfrak h)^W$, độc lập với lựa chọn của $B$.

a) Cho $P_{++}$ là tập hợp các trọng số trội của $R$, $w\in W$, $\lambda\in P_{++}$, $\mu=w\lambda$. Khi đó $Z(\mu-\rho)$ đẳng cấu với một môđun con của $Z(\lambda-\rho)$ (§6, no. 3, Hệ quả 2 của Mệnh đề 6), và $\varphi(u)(\lambda-\rho)=\varphi(u)(\mu-\rho)$ với mọi $u\in Z$ (§6, no. 4, Mệnh đề 7). Do đó, các hàm đa thức $(\delta\circ\varphi)(u)$ và $(\delta\circ\varphi)(u)\circ w$ trên $\mathfrak h^*$ trùng nhau trên $P_{++}$. Nhưng $P_{++}$ là *trù mật* trong $\mathfrak h^*$ đối với tôpô Zariski: điều này có thể thấy được bằng cách đồng nhất $\mathfrak h^*$ với $k^B$ nhờ cơ sở gồm các trọng số cơ bản $\varpi_\alpha$, và bằng cách áp dụng Mệnh đề 9 của *Đại số*, Chap. IV, §2, no. 3. Do đó

$$
(\delta\circ\varphi)(u)=(\delta\circ\varphi)(u)\circ w,
$$

điều này chứng minh rằng $(\delta\circ\varphi)(Z)\subset S(\mathfrak h)^W$.

b) Cho $\eta$ là đẳng cấu từ $I(\mathfrak g)$ đến $S(\mathfrak h)^W$ được xác định trong no. 3, Hệ quả 2 của Định lý 1. Xét đẳng cấu chính tắc từ $\mathfrak g$-môđun $U$ đến $\mathfrak g$-môđun $S(\mathfrak g)$ (Chap. I, §2, no. 8), và cho $\theta$ là hạn chế của nó lên $Z$. Khi đó $\theta(Z)=I(\mathfrak g)$. Cho $z$ là một phần tử của $Z$ có lọc $\leqslant f$ trong $U$.

$$
\begin{array}{ccc}
Z & \xrightarrow{\theta} & I(\mathfrak g)\\
\Big\downarrow{\scriptstyle\varphi} & & \Big\downarrow{\scriptstyle\eta}\\
S(\mathfrak h) & \xrightarrow{\delta} & S(\mathfrak h).
\end{array}
$$

Đưa vào các ký hiệu của §6, no. 4, và đặt

$$
z=
\sum_{\sum q_i+\sum m_i+\sum p_i\leqslant f}
\lambda_{(q_i),(m_i),(p_i)}
u((q_i),(m_i),(p_i)).
$$

Cho $v((q_i),(m_i),(p_i))$ là đơn thức
$X_{\alpha_1}^{q_1}\cdots X_{\alpha_n}^{q_n}H_1^{m_1}\cdots H_l^{m_l}X_{\alpha_1}^{p_1}\cdots X_{\alpha_n}^{p_n}$
được tính trong $S(\mathfrak g)$. Ký hiệu $S_d(\mathfrak g)$ là tổng của các thành phần thuần nhất của $S(\mathfrak g)$ có các bậc $0,1,\ldots,d$, ta có

$$
\theta(z)\equiv
\sum_{\sum q_i+\sum m_i+\sum p_i=f}
\lambda_{(q_i),(m_i),(p_i)}v((q_i),(m_i),(p_i))
\pmod{S_{f-1}(\mathfrak g)}
$$

nên

$$
(\eta\circ\theta)(z)\equiv
\sum_{\sum m_i=f}
\lambda_{(0),(m_i),(0)}v((0),(m_i),(0))
\pmod{S_{f-1}(\mathfrak h)}
$$

và do đó

$$
(\eta\circ\theta)(z)\equiv\varphi(z)
\pmod{S_{f-1}(\mathfrak h)}.
\tag{3}
$$

c) Ta chứng minh rằng $\delta\circ\varphi:Z\longrightarrow S(\mathfrak h)^W$ là song ánh. Các lọc chính tắc trên $U$ và $S(\mathfrak g)$ cảm sinh các lọc trên $Z$, $I(\mathfrak g)$ và $S(\mathfrak h)^W$, và $\theta$, $\eta$ tương thích với các lọc này, sao cho gr($\eta \circ \theta$ ) là một đẳng cấu từ không gian vectơ gr(Z) đến không gian vectơ gr($\mathbf{S}(\mathfrak{h})^W$). Theo (3), gr($\varphi$ ) $=$ gr($\eta \circ \theta$ ), và hiển nhiên rằng gr($\delta$ ) là đồng nhất. Do đó gr($\delta \circ \varphi$ ) là song ánh, nên

$$
\delta \circ \varphi : Z\rightarrow \mathbf{S}(\mathfrak{h})^W
$$

là song ánh (Đại số giao hoán, Chương III, §2, no. 8, Hệ quả 1 và 2 của Định lý 1).

d) Nhắc lại các ký hiệu trong a). Cho E là một $\mathfrak{g}$-môđun đơn có trọng số cao nhất $\lambda$, và $\chi$ là đặc trưng trung tâm của nó (§6, no. 1, Định nghĩa 2). Gọi $\varphi '$ và $\delta '$ là các đồng cấu tương tự với $\varphi$ và $\delta$ tương ứng với cơ sở $w(B)$. Trọng số cao nhất của E tương ứng với $w(B)$ là $w(\lambda )$. Theo §6, no. 4, Mệnh đề 7,

$$
\varphi (u)(\lambda ) =\chi (u) =\varphi '(u)(w\lambda )
$$

với mọi $u\in Z$, nên, theo a),

$$
(\delta \circ \varphi )(u)(w\lambda +w\rho ) = (\delta \circ \varphi )(u)(\lambda +\rho ) =\varphi (u)(\lambda ) =\varphi '(u)(w\lambda )
$$

$$
= (\delta '\circ \varphi ')(u)(w\lambda +w\rho )
$$

Do đó, các hàm đa thức $(\delta \circ \varphi )(u)$ và $(\delta '\circ \varphi ')(u)$ trùng nhau trên $w(P_{++}) +w\rho$, và vì thế bằng nhau.

#### Hệ quả 1 {#lie-viii-s8-thm-2-cor-1 .statement tag=015K}

Với mọi $\lambda \in \mathfrak{h}^*$, đặt $\chi_{\lambda}$ là đồng cấu $z \rightarrow (\varphi (z))(\lambda )$ từ Z vào $k$.

(i) Nếu $k$ đóng đại số, mọi đồng cấu từ Z vào $k$ đều có dạng $\chi_{\lambda}$ với một $\lambda \in \mathfrak{h}^*$ nào đó.

(ii) Cho $\lambda , \mu\in \mathfrak{h}^*$. Khi đó $\chi_{\lambda}=\chi_\mu$ khi và chỉ khi $\mu+\rho \in W(\lambda +\rho )$.

Nếu $k$ là đóng đại số, mọi đồng cấu từ $\mathbf{S}(\mathfrak{h})^W$ vào $k$ đều mở rộng được thành một đồng cấu từ $\mathbf{S}(\mathfrak{h})$ vào $k($Đại số giao hoán, Ch. V, §1, no. 9, Mệnh đề 22, và §2, no. 1, Hệ quả 4 của Định lý 1), và mọi đồng cấu từ $\mathbf{S}(\mathfrak{h})$ vào $k$ đều có dạng $f \rightarrow f(\lambda )$ với một $\lambda \in \mathfrak{h}^*$ nào đó (Ch. VII, Phụ lục I, Mệnh đề 1). Do đó, nếu $\chi$ là một đồng cấu từ Z vào $k$, tồn tại (Định lý 2) một $\mu\in \mathfrak{h}^*$ sao cho, với mọi $z\in Z$,

$$
\chi (z) = ((\delta \circ \varphi )(z))(\mu) = (\varphi (z))(\mu-\rho )
$$

suy ra (i).

Cho $\lambda , \mu\in \mathfrak{h}^*$ và giả sử rằng $\chi_{\lambda}=\chi_\mu$. Khi đó, với mọi $z\in Z$,

$$
((\delta \circ \varphi )(z))(\lambda +\rho ) = (\varphi (z))(\lambda ) =\chi_{\lambda}(z) =\chi_\mu(z) = ((\delta \circ \varphi )(z))(\mu+\rho )
$$

nói cách khác, các đồng cấu từ $\mathbf{S}(\mathfrak{h})$ vào $k$ được xác định bởi $\lambda +\rho$ và $\mu+\rho$ trùng nhau trên $\mathbf{S}(\mathfrak{h})^W$; do đó, mệnh đề (ii) suy ra từ Đại số giao hoán, Ch. V, §2, no. 2, Hệ quả của Định lý 2.

#### Hệ quả 2 {#lie-viii-s8-thm-2-cor-2 .statement tag=015L}

Cho $E,E'$ là các $\mathfrak{g}$-môđun đơn hữu hạn chiều, và $\chi , \chi '$ là các ký tự trung tâm của chúng. Nếu $\chi =\chi '$, E và $E'$ đẳng cấu.

Cho $\lambda , \lambda '$ là các trọng cao nhất của $E,E'$. Theo §6, no. 4, Mệnh đề $7,\chi_{\lambda}=\chi =$ $\chi '=\chi_{\lambda'}$, do đó tồn tại $w\in W$ sao cho $\lambda '+\rho =w(\lambda +\rho )$. Vì $\lambda +\rho$ và $\lambda '+\rho$ thuộc buồng được xác định bởi B, ta có $w= 1$. Vậy, $\lambda =\lambda '$, do đó có hệ quả.

#### Mệnh đề 7 {#lie-viii-s8-prop-7 .statement tag=015M}

Với mọi lớp $\gamma$ của các $\mathfrak{g}$-môđun đơn hữu hạn chiều, gọi $U_{\gamma}$ là thành phần đẳng kiểu kiểu $\gamma$ của $\mathfrak{g}$-môđun U (đối với biểu diễn phụ hợp của $\mathfrak{g}$ trên U). Gọi $\gamma_0$ là lớp của $\mathfrak{g}$-môđun tầm thường chiều 1. Gọi $[U,U]$ là không gian con vectơ của U sinh bởi các móc của các cặp phần tử của U.

(i) U là tổng trực tiếp của các $U_{\gamma}$.

(ii) $U_{\gamma_0}= Z$, và $\sum_{\gamma\not=\gamma_0}U_{\gamma}= [U,U]$.

(iii) Gọi $u \rightarrow u^{\natural}$ là phép chiếu của U lên Z được xác định bởi phân tích $U = Z\oplus [U,U]$. Nếu $u\in U$ và $v\in U$, ta có $(uv)^{\natural}= (vu)^{\natural}$. Nếu $u\in U$ và $z\in Z$, ta có $(uz)^{\natural}=u^{\natural}z$.

(iv) Cho $\varphi$ là đồng cấu Harish-Chandra. Cho $\lambda \in P_{++}$, và cho E là một $\mathfrak{g}$-môđun đơn hữu hạn chiều có trọng số cao nhất là $\lambda$. Với mọi $u\in U$, ta có

dim E1 Tr($u_E$) $= (\varphi (u^{\natural}))(\lambda )$.

$\mathfrak{g}$-môđun U là một tổng trực tiếp của các môđun con hữu hạn chiều. Điều này suy ra (i).

Rõ ràng $U_{\gamma_0}= Z$. Gọi $U'$ là một không gian con vectơ của U xác định một biểu diễn con thuộc lớp $\gamma$ của biểu diễn phụ hợp. Khi đó hoặc là $[\mathfrak{g},U'] = U'$ hoặc là $[\mathfrak{g},U'] = 0$. Do đó, nếu $\gamma \not=\gamma_0$ thì $[\mathfrak{g},U'] = U'$, suy ra $\sum_{\gamma\not=\gamma_0}U_{\gamma}\subset [U,U]$. Mặt khác, nếu $u\in U$ và $x_1, . . . , x_n\in \mathfrak{g}$, thì

$$
[x_1. . . x_n, u] = (x_1. . . x_nu-x_2. . . x_nux_1)+(x_2. . . x_nux_1-x_3. . . x_nux_1x_2)
$$

$$
+\cdots + (x_nux_1. . . x_{n-1}-ux_1. . . x_n)\in [\mathfrak{g},U]
$$

Suy ra $[U,U]\subset [\mathfrak{g},\sum_{\gamma}U_{\gamma}]=[\mathfrak{g},\sum_{\gamma\not=\gamma_0}U_{\gamma}]\subset \sum_{\gamma\not=\gamma_0}U_{\gamma}$. Điều này chứng minh (ii). Với các điều kiện này, (iii) suy ra từ Chap. I, §6, no. 9, Bổ đề 5.

Cuối cùng, cho $E, \lambda$ như trong (iv). Khi đó

Tr($u_E$) $=$ Tr(($u^{\natural}$)$_E$) vì $u-u^{\natural}\in [U,U]$

= Tr($\varphi (u^{\natural})(\lambda ).1$) (§$6$, no$.4$, Prop$.7$)

= (dim $E$)$.\varphi (u^{\natural})(\lambda )$.

### Bài tập {#lie-viii-s8-exercises}

Xem [các bài tập cho § 8](exercises/s8/).
